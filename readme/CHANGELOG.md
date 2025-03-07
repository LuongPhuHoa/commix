## Version 3.0 (upcoming)
* Revised: Improvement regarding identifying the indicated web-page charset.
* Added: Support for Python 3.x
* Updated: Beautiful Soup (third party) module has been updated.
* Added: Six (third party) module has been added.
* Revised: Improvement regarding parsing nested JSON objects that contain boolean values.
* Replaced: The `--ignore-401` option has been replaced with `--ignore-code` option.
* Added: New option ( `--ignore-code`) for ignoring (problematic) HTTP error code (e.g. 401).

## Version 2.9 (2019-06-26)
* Fixed: Multiple bug-fixes regarding several reported unhandled exceptions.
* Fixed: Bug-fix regarding parsing hostname and port from URL.
* Revised: Improvement regarding automatically decoding "deflate" and "gzip" HTTP responses.
* Fixed: Bug-fix regarding parsing HTTP header values that contain multiple ":".
* Revised: Improvement regarding updating "Content-Length" HTTP header, in case it's provided by user (i.e. `-r`, `--header`, `--header` options).
* Revised: Improvement regarding parsing raw HTTP headers from a file (i.e. `-r` option).
* Revised: Improvement regarding parsing nested JSON objects.
* Added: Flatten_json (third party) module has been added.
* Revised: Bug-fixes and improvements regarding parsing JSON objects.
* Added: GPL Cooperation Commitment (COMMITMENT.txt) has been added.
* Updated: Minor update regarding HTTP authentication (Basic / Digest).
* Revised: Minor improvements regarding preventing false negative results, due to parameters tampering during the detection phase.
* Revised: Minor improvements regarding "reverse_tcp" and "bind_tcp" shell options.

## Version 2.8 (2019-03-26)
* Fixed: Multiple bug-fixes regarding several reported unhandled exceptions.
* Updated: Minor update regarding accepting overly long result lines.
* Revised: Minor bug-fixes and improvements regarding `--file-upload` option.
* Revised: Minor bug-fixes and improvements regarding HTTP authentication dictionary-based cracker.
* Revised: Minor bug-fixes and improvements regarding HTTP authentication (Basic / Digest).
* Fixed: Minor bug-fix regarding ignoring HTTP Error 401 (Unauthorized) (for `--ignore-401` option).
* Added: Support for writing crawling results to a temporary file (for eventual further processing with other tools).
* Added: Support for Windows "Python" on "reverse_tcp" shell option.

## Version 2.7 (2018-12-18)
* Fixed: Multiple bug-fixes regarding several reported unhandled exceptions.
* Revised: The suffixes list has been shortly revised.
* Updated: With each commix run end users are obligated to agree with the "Legal disclaimer" prelude message.
* Fixed: Minor improvent regarding local HTTP server (for `--file-upload` option).
* Added: A list of extensions to exclude from crawling.
* Revised: Minor improvements regarding crawler.
* Revised: Minor update of redirection mechanism.
* Revised: Minor improvement regarding identifying the target web server.
* Revised: Minor improvement regarding identifying corrupted .pyc file(s).
* Added: New tamper script "dollaratsigns.py" that adds dollar-sign followed by an at-sign ("$@") between the characters of the generated payloads.
* Fixed: Bug-fix regarding proxying SSL/TLS requests.
* Revised: Minor improvement regarding checking for potentially miswritten (illegal '=') short option.
* Revised: Minor improvement regarding checking for illegal (non-console) quote and comma characters.
* Revised: Minor improvement regarding merging of tamper script arguments.
* Revised: Minor improvement regarding ignoring the parameter(s) that carrying anti-CSRF token(s) in all scanning attempts.
* Updated: Beautiful Soup (third party) module has been updated.
* Added: New tamper script "xforwardedfor.py" that appends a fake HTTP header 'X-Forwarded-For'.
* Fixed: Minor bug-fix regarding loading tamper scripts. 
* Revised: Minor improvement regarding "INJECT_HERE" tag (i.e. declaring injection position) to be case insensitive.

## Version 2.6 (2018-09-21)
* Fixed: Multiple bug-fixes regarding several reported unhandled exceptions.
* Revised: Minor improvement in session handler regarding IPv6 targets.
* Added: New option `--list-tampers` for listing available tamper scripts.
* Revised: Minor improvement regarding resolving target hostname.
* Added: Support for "Ncat" on "reverse_tcp" and "bind_tcp" shell options.
* Added: Support for "Bash" (via /dev/tcp) on "reverse_tcp" shell option.
* Added: Support for "Netcat-Openbsd" (nc without -e) on "reverse_tcp" and "bind_tcp" shell options.
* Added: Support for "Socat" on "reverse_tcp" and "bind_tcp" shell options.
* Revised: Minor improvement regarding counting the total of HTTP(S) requests, for the identified injection point(s) during the detection phase.
* Fixed: Minor bug-fix regarding providing the target host's root directory.
* Added: New tamper script "sleep2timeout.py" that uses "timeout" function for time-based attacks.
* Added: New tamper script "sleep2usleep.py" that replaces "sleep" with "usleep" command in the time-related generated payloads.
* Replaced: The `--purge-output` option has been replaced with `--purge` option.
* Fixed: Minor bug-fix regarding performing injections through cookie parameters.
* Revised: Minor improvement regarding ignoring the Google Analytics cookie in all scanning attempts.
* Fixed: Minor bug-fix regarding "bind_tcp" shell option.

## Version 2.5 (2018-07-13)
* Fixed: Multiple bug-fixes regarding several reported unhandled exceptions.
* Revised: Improvement regarding identifying the appropriate format parameters, in the provided POST data.
* Added: Support regarding recognition of generic "your ip has been blocked" messages.
* Added: Support regarding checking for potential browser verification protection mechanism.
* Added: Support regarding checking for potential CAPTCHA protection mechanism.
* Revised: The separators list, has been shortly revised.
* Revised: Minor improvement regarding the extracted HTTP response headers.
* Added: New tamper script "nested.py" that adds double quotes around of the generated payloads (for *nix targets).
* Fixed: Minor bug-fix regarding performing injections through HTTP Headers (e.g User-Agent, Referer, Host etc).
* Fixed: Major bug-fixes regarding testing time-related ("time-based"/"tempfile-based") payloads.
* Added: New tamper script "backslashes.py" that adds back slashes (\) between the characters of the generated payloads (for *nix targets).
* Fixed: Minor bug-fix regarding unicode decode exception error due to invalid codec, during connection on target host.
* Revised: Improvement regarding combining tamper script "multiplespaces.py" with other space-related tamper script(s).
* Added: New tamper script "multiplespaces.py" that adds multiple spaces around OS commands.

## Version 2.4 (2018-05-21)
* Fixed: Multiple bug-fixes regarding several reported unhandled exceptions. 
* Fixed: Minor bug-fix regarding ignoring invalid and/or empty tamper scripts. 
* Updated: Colorama (third party) module has been updated.
* Revised: Minor improvement regarding keeping the git folder 'clean' (via @g0tmi1k).
* Fixed: Minor bug-fix regarding loading multiple tamper scripts (during the exploitation phase). 
* Added: New tamper script "caret.py" that adds the caret symbol (^) between the characters of the generated payloads (for windows targets).
* Added: New tamper script "singlequotes.py" that adds single quotes (') between the characters of the generated payloads (for *nix targets).

## Version 2.3 (2018-03-07)
* Fixed: Multiple bug-fixes regarding several reported unhandled exceptions. 
* Revised: Minor improvement regarding testing the Host HTTP header.
* Added: Support for Host HTTP header command injections.
* Revised: Minor improvement regarding testing SOAP/XML POST data.
* Added: Support for automatically creating a Github issue with unhandled exception information.
* Revised: Improvement for masking sensitive data in the detailed message about occurred unhandled exception.
* Added: Support for returning detailed message about occurred unhandled exception.
* Revised: The `--charset` option has been revised to force the usage of custom charset in order to speed-up the data retrieval process (during time-related injections).
* Replaced: The `--charset` option has been replaced with `--encoding` option.
* Revised: Improvement regarding batch mode, for testing the payloads for both OS - if it's not able to identify the target OS.
* Added: Support for SOAP/XML POST data.
* Fixed: Bug-fix regarding the SSL implementation (via @TD4B). 
* Revised: Improvement regarding testing json-formated POST data with empty value(s).
* Revised: Minor improvement regarding verbose mode for removing the first and/or last line of the html content (in case there are/is empty).

## Version 2.2 (2017-12-12)
* Revised: Minor improvement in "updater", for supporting verbose mode.
* Fixed: Minor bug-fix regarding cookie-based command injections.
* Revised: Minor improvement regarding option `-p` for bypassing the dependence on value of `--level` (in case of user-defined HTTP headers).
* Revised: Minor improvement regarding option `-p` for testing user-defined HTTP headers.
* Added: New option `--failed-tries` for setting a number of failed injection tries, in file-based technique.
* Revised: Minor improvement regarding session handler.
* Revised: Minor improvement regarding checking stored time-related ("time-based"/"tempfile-based") payloads.
* Revised: Minor improvement regarding Python version check (no more crashes on Python >= "3" and < "2.6").
* Revised: Minor improvement in "updater", for checking commit hash number.
* Added: New option `--skip` regarding excluding certain parameter(s) from testing.
* Added: New option `--skip-technique` regarding excluding certain injection technique(s) from testing.

## Version 2.1 (2017-10-03)
* Added: New option `--header` for providing a single extra HTTP header (e.g. 'X-Forwarded-For: 127.0.0.1').
* Added: New option `--check-internet` that checks internet connection before assessing the target.
* Fixed: Minor bug-fix regarding performing injections through HTTP Headers (i.e Cookie, User-Agent, Referer).
* Revised: Minor improvement regarding checking stored payloads and enabling appropriate tamper scripts during the exploitation phase.
* Added: New tamper script "space2vtab.py" that replaces every space ("%20") with vertical tab ("%0b") (for Windows targets).
* Replaced: The tamper script "space2tab.py" has been replaced with "space2htab.py".
* Fixed: Minor bug-fix regarding checking for similarity in provided parameter name and value (GET / POST).
* Added: New option `--backticks` that uses backticks instead of "$()", for commands substitution.
* Revised: Minor improvement in Netcat shells, for giving to the end-user the choice of using the "/bin" standard subdirectory.
* Added: New option `--disable-coloring` that disables console output coloring.
* Added: New option `--check-tor` that checks if Tor is used properly.
* Fixed: Minor improvement for fetching random HTTP User-Agent header in initial request, when `--random-agent` is used.
* Revised: Minor improvement regarding options `--purge-output` and `--wizard`, were added in the mandatory options list.
* Fixed: Major bug-fix regarding connection problem over HTTPS.
* Added: New option `--purge-output` to turn on safe removal of all content(s) from output directory.

## Version 2.0 (2017-07-14)
* Revised: Minor improvement for automatically increasing default `--time-sec` value when `--tor` used.
* Fixed: Minor improvement for not re-testing Tor SOCKS proxy settings (in case of multiple targets).
* Revised: Multiple minor eye-candy revisions have been performed.
* Fixed: Major improvement regarding not sending requests with GET mothod in case of POST method, in injection levels 2, 3.
* Updated: The `--sys-info` option has been enriched with distribution description and release information.  
* Revised: Minor improvement in dynamic code evaluation, regarding the users extraction payload. 
* Fixed: Minor fix regarding not raising the detection phase in the case of 4xx and/or 5xx HTTP error codes.
* Revised: Minor improvement regarding not re-performing requests in case of stored session.
* Revised: Minor improvement in time-related techinques for checking the reliability of the used payload (in case of a false positive result).
* Updated: Minor update in the list of the User-Agents (regarding the `--random-agent` option).
* Added: New option `--mobile` that imitates smartphone through HTTP User-Agent header.
* Added: New option `--retries` that retries request(s) when the connection timeouts.

## Version 1.9 (2017-05-02)
* Revised: Minor improvement in results-based techniques, for delaying the OS responses depending on the user-provided time delay.
* Revised: The time-related ("time-based"/"tempfile-based") payloads, have been shortly revised.
* Revised: Minor improvement in file-based technique, for delaying the OS responses depending on the user-provided time delay.
* Fixed: Minor improvement in file-based technique, regarding τhe directory path that the output file is saved.
* Added: New option `--ignore-redirects` that ignoring redirection attempts.
* Added: New functionality for identifying and following URL redirections.
* Fixed: Minor improvement for adding "/" at the end of the user provided root dir (in case it does not exist).
* Revised: The file-based payload for deleting files with execution output, has been shortly revised.
* Replaced: The `--root-dir` option has been replaced with `--web-root` option.
* Added: New option `--wizard` that shows a simple wizard interface for beginner users.

## Version 1.8 (2017-03-15)
* Added: New feauture for installing Unicorn tool (if not installed on host).
* Removed: The pre-installed version of Unicorn tool has been removed.
* Added: New feauture for checking and updating current version of Unicorn tool.
* Revised: The `--delay` option has been revised to delay between each HTTP request.
* Replaced: The `--delay` option has been replaced with `--time-sec` option.
* Fixed: Minor improvement regarding gnureadline module for better support on MacOS X hosts.
* Added: New option `--charset` that forces character encoding used for data retrieval.
* Added: New prefix ("'%26") and suffix ("%26'") have been added.
* Fixed: Removal of unnecessary command substitution in semiblind ("file-based") technique.
* Updated: The Unicorn tool has been updated to version 2.4.2.
* Added: Support for the Regsvr32.exe Application Whitelisting Bypass technique.
* Fixed: Minor improvement for checking for established TCP connections.
* Fixed: Minor improvement for not reopening meterpreter sessions (in case of user abortion).

## Version 1.7 (2017-02-03)
* Fixed: Minor improvement regarding unverified SSL context(s).
* Added: New values ("URIPATH", "SRVPORT") have been added to "Set" option.
* Revised: Minor improvements regarding "reverse_tcp" and "bind_tcp" shell options.
* Fixed: Minor improvement for checking missing mandatory option(s).
* Fixed: Minor improvement regarding the file path of the null device.
* Fixed: Minor improvement regarding automated scan level increasing.
* Fixed: Improvement regarding skipping the testing of problematic URL(s) and proceeding with next ones (in case of scanning multiple targets). 
* Fixed: Improvement regarding printing current assessment state in case of user abortion. 
* Revised: Minor improvement for proceeding with semiblind ("file-based") technique, once the user provides the path of web server's root directory.
* Fixed: Minor fix regarding the lack of http/s to the user-defined URL(s).
* Added: New option `--skip-empty` for skipping the testing of the parameter(s) with empty value(s).
* Fixed: Improvement regarding testing the parameter(s) with empty value(s).
* Added: New CGI shellscript path "/cgi-bin/cgiCmdNotify" (vulnerable to shellshock) has been added.

## Version 1.6 (2016-12-28)
* Fixed: Improvement regarding json-formated POST data, where whitespace before (and/or after) the ":" exists.
* Fixed: Minor fix regarding empty value(s) in provided parameter(s).
* Added: New option `--batch` that never asks for user input (using the default behaviour).
* Added: New option `-x` for parsing target(s) from remote sitemap(.xml) file.
* Added: New option `--offline` for working in offline mode.
* Fixed: Improvement regarding the IP address grabbing (in case of internet in-accessibility).
* Fixed: Improvement regarding HTTPS based websites, for which scanning fails.
* Added: New option `-r` for loading HTTP request from a file.
* Fixed: Improvement regarding the response time estimimation, in which the target URL was requested without its POST data.
* Added: New option `-m` for scanning multiple targets given in a textual file.
* Fixed: Minor fix regarding the newline display in dynamic code evaluation ("eval-based") and semiblind ("file-based") technique.
* Revised: The dynamic code evaluation ("eval-based") payloads have been shortly revised.
* Added: The executed command and the execution results output has been added to log file.

## Version 1.5 (2016-11-17)
* Fixed: Minor improvement in the "ICMP exfiltration" module.
* Fixed: Minor improvement for choosing default value when pressing enter.
* Added: New tamper script "hexencode.py" that encodes the payload to hex format.
* Fixed: Minor improvements in executed commands history.
* Added: New verbosity level (4) for printing the HTTP response page content.
* Added: New option `-t` for logging all HTTP traffic into a textual file.
* Added: New option `--msf-path` for specifying a path where metasploit is installed.
* Added: New verbosity level (3) for printing the HTTP response headers.
* Added: New verbosity level (2) for printing the performed HTTP requests headers.

## Version 1.4 (2016-10-17)
* Added: Support on crawler for checking target for the existence of 'sitemap.xml'.
* Revised: The payload for Ruby reverse-shell has been shortly revised.
* Added: Support for bind TCP shell (via "bind_tcp" option).
* Added: New option `--crawl` (1,2) for crawling of a given website, starting from the target url.
* Updated: The Unicorn tool has been updated to version 2.3.5.
* Added: The project's official URL has been added in the menu banner.
* Fixed: Minor improvements in tab completion.
* Fixed: Minor improvement in the function that checks for updates on start up.
* Fixed: Minor improvements in enumeration options (added failure messages).

## Version 1.3 (2016-09-14)
* Fixed: Minor improvements in "reverse_tcp" option.
* Added: Support for the metasploit "web_delivery" script.
* Added: Support for generating Python/PHP meterpreter reverse TCP payloads via metasploit.
* Fixed: Minor improvements for enumeration options (if `--url-reload` is used).
* Added: The ability for generating and injecting native x86 shellcode (Powershell).
* Added: New option `--skip-calc` that skips the mathematic calculation during the detection phase.
* Fixed: Minor improvement in Shellshock module for ignoring junk output on response.
* Fixed: Minor improvement in Shellshock module for finding RCE results on page's response.

## Version 1.2 (2016-08-12)
* Added: The ability for setting custom (PHP / Python) working directory.
* Fixed: License file minor inaccurancy issue has been fixed.
* Revised: The Windows-based payloads for every supported technique, had been shortly revised.
* Revised: The dynamic code evaluation ("eval-based") technique has been shortly revised.
* Added: New tamper script "space2tab.py" that replaces every space ("%20") with horizontal tab ("%09").
* Added: The ability for generating powershell attack vectors via TrustedSec's Magic Unicorn.
* Added: The ability for checking if there is a new version available.
* Added: The ability for target application extension recognition (i.e PHP, ASP etc).
* Fixed: Minor improvement for finding the URL part (i.e scheme:[//host[:port]][/]path).
* Fixed: Minor fix for conflicted shells (i.e regular, alternative) from session file.

## Version 1.1 (2016-07-14)
* Added: The ".gitignore" file has been added.
* Added: Support for injections against ASP.NET applications.
* Added: Support for warning detection regarding "create_function()" function.
* Fixed: Minor improvent of the HTTP server for `--file-upload` option.
* Fixed: Minor fix for conflicted executed commands from session file in HTTP Headers.
* Added: The ability to store injection level into session files for current target. 
* Added: Support for automated enabling of an HTTP server for `--file-upload` option.
* Fixed: Minor fix for "Python-urllib" User-Agent exposure.

## Version 1.0 (2016-06-14)
* Revised: Time-relative statistical analysis for recognition of unexpected time delays due to unstable requests.
* Added: A list of pages / scripts potentially vulnerable to shellshock.
* Added: The ability to check if the url is probable to contain script(s) vulnerable to shellshock.
* Revised: Multiple eye-candy revisions have been performed.
* Fixed: HTTPS requests fixation, if the `--proxy` option is enabled.
* Fixed: Multiple fixes regarding the shellshock module have been performed.

## Version 0.9b (2016-06-07)
* Added: The ability to re-perform the injection request if it has failed.
* Fixed: The shell output in semiblind ("file-based") technique has been fixed not to concat new lines.
* Revised: The ability to execute multiple tamper scripts combined or the one after the other.
* Added: New tamper script "space2plus.py" that replaces every space ("%20") with plus ("+").
* Added: New state ("checking") and the color of that state has been setted.
* Replaced: The `--base64` option has been replaced with "base64encode.py" tamper script.
* Added: New tamper script "space2ifs.py" that replaces every space ("%20") with $IFS (bash) variable.
* Added: New option `--tamper` that supports tamper injection scripts.
* Added: Support for verbosity levels (currently supported levels: 0,1).
* Fixed: Minor rearrangement of prefixes and separators has been implemented.
* Revised: The "time-based" (blind) technique for *nix targets has been shortly revised.
* Revised: The source code has been revised to support "print_state_msg" (i.e error, warning, success etc) functions.

## Version 0.8b (2016-05-06)
* Fixed: The `--file-read` option to ignore the carriage return ("\r") character in a text file.
* Added: The ability to check for empty value(s) in the defined GET/POST/Cookie(s) data and skip.
* Replaced: The "INJECT_HERE" tag has been replaced with the "*" (asterisk) wildcard character.
* Added: New option `--level` (1-3) that specifies level of tests to perform.
* Added: New option `-p` that specifies a comma-separated list of GET/POST parameter.
* Added: The ability to check every parameter in the provided cookie data.
* Added: The ability to check every GET parameter in the defined URL and/or every POST provided data.
* Added: New option `--all` that enables all supported enumeration options.

## Version 0.7b (2016-04-18)
* Fixed: HTTP proxy logs parser to accept GET http requests.
* Fixed: HTTP proxy logs parser to recognise provided HTTP authentication credentials.
* Added: Support for verbose mode in HTTP authentication (Basic / Digest) dictionary-based cracker.
* Added: The ability to store valid (Digest) credentials into session files for current target.
* Added: Dictionary-based cracker for "Digest" HTTP authentication credentials.
* Added: Support for "Digest" HTTP authentication type.

## Version 0.6b (2016-04-01)
* Added: The ability to store valid (Basic) credentials into session files for current target.
* Added: New option `--ignore-401` that ignores HTTP Error 401 (Unauthorized) and continues tests without providing valid credentials.
* Added: Dictionary-based cracker for "Basic" HTTP authentication credentials.
* Added: Identifier for HTTP authentication type (currently only "Basic" type is supported).
* Added: New option `--skip-waf` that skips heuristic detection of WAF/IPS/IDS protection.
* Added: Support for verbose mode in the "DNS exfiltration" injection technique (module).
* Added: New option `--dns-server` that supports the "DNS exfiltration" injection technique (module).
* Added: New option `--dependencies` that checks (non-core) third party dependenices.

## Version 0.5b (2016-03-16)
* Fixed: The payload(s) for dynamic code evaluation ("eval-based"), if there is not any separator.
* Added: Support for verbose mode in the "ICMP exfiltration" injection technique (module). 
* Added: Check if the user-defined os name, is different than the one identified by heuristics.
* Added: New option `--os` that forces a user-defined os name.
* Added: Support for testing custom HTTP headers (via `--headers` parameter).

## Version 0.4.1b (2016-02-26)
* Added: Support for storing and retrieving executed commands from session file.
* Added: New option `-s` for loading session from session file.
* Added: New option `--ignore-session` for ignoring results stored in session file.
* Added: New option `--flush-session` for flushing session files for current target.
* Added: Support to resume to the latest injection points from session file.

## Version 0.4b (2016-02-04)
* Added: Payload mutation if WAF/IPS/IDS protection is detected.
* Added: Check for existence of WAF/IPS/IDS protection (via error pages).
* Added: The "set" option in "reverse_tcp" which sets a context-specific variable to a value.
* Added: New option `--force-ssl` for forcing usage of SSL/HTTPS requests.

## Version 0.3b (2016-01-15)
* Added: Time-relative false-positive identification, which identifies unexpected time delays due to unstable requests.
* Added: New option `-l`, that parses target and data from HTTP proxy log file (i.e Burp or WebScarab).
* Added: Check if Powershell is enabled in target host, if the applied option's payload is requiring the use of PowerShell.
* Added: New option `--ps-version`, that checks PowerShell's version number.
* Replaced: Some powershell-based payloads, have been replaced by new (more solid) ones, so to avoid "Microsoft-IIS" server's incompatibilities.
* Added: Support (in MacOSX platforms) for a tab completion in shell options.
* Added: Undocumented parameter "-InputFormat none" so to avoid "Microsoft-IIS" server's hang.
* Added: Ability for identification of "Microsoft-IIS" servers.
* Added: Statistical checks for time-related ("time-based"/"tempfile-based") techniques.
* Added: Support for Windows-based (cmd / powershell) payloads for every injection technique.

## Version 0.2b (2015-12-18)
* Added: Support for recalling previous commands.
* Added: Support (in Linux platforms) for tab completion in shell options.
* Added: Support for alternative (Python) os-shell in dynamic code evaluation ("eval-based") technique.
* Added: Support for PHP/Python meterpreter on "reverse_tcp" shell option.
* Added: The "reverse_tcp" shell option.
* Added: The ability to check for default root directories (Apache/Nginx).
* Added: Support for removal of (txt) shell files in semiblind ("file-based"/"tempfile-based") techniques.
* Added: Support for JSON POST data.
* Added: The "enumeration" and "file-read" results to log file.
* Added: The ability to get the user's approval before re-{enumerate/file-read} target.
* Added: The ability to stop current injection technique and proceed on the next one(s).

## Version 0.1b (2015-09-20)
* Added: New eval-based payload for "str_replace()" filter bypass.
* Added: Check for (GET) RESTful URL format.
* Added: New option `--base64`, that encodes the OS command to Base64 format. 
* Added: Support for regular "preg_replace()" injections via "/e" modifier.
* Added: Support for HTML Charset and HTTP "Server" response-header reconnaissance (on verbose mode).
* Replaced: Payloads for "tempfile-based" (semiblind) technique, have been replaced by new (more solid) ones.
* Added: A "new-line" separator support, for "time-based" (blind) & "tempfile-based" (semiblind) techniques.
* Added: Support for Referer HTTP header command injections.
* Added: Support for User-Agent HTTP header command injections.
* Added: CVE-2014-6278 support for "shellshock" module.
* Added: Support for cookie-based command injections.
* Added: A generic false-positive prevention technique.
* Removed: The "Base64" detection option.
* Added: Support for the Tor network.
* Added: The "shellshock" (CVE-2014-6271) injection technique (module).
* Added: Termcolor support for Windows (colorama).
* Added: File access options.
* Added: Enumeration options.
* Added: New option `--alter-shell` that supports an alternative option for os-shell (e.g. Python).
* Added: New option `--icmp-exfil` that supports the "ICMP exfiltration" injection technique (module).
* Added: The "tempfile-based" (semiblind) technique.
* Added: The "file-based" (semiblind) technique.
* Removed: The "boolean-based" (blind) technique.
* Added: More Options.

## Version 0.1a (2014-12-20)
* The initial release {aka the Birth!}.
