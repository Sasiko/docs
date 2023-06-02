# URL List

## How URL List works

Some malicious actors on discord are using legitimate website as file storage purpose. They will later use those site to serve as direct download links. The issue with direct download links is that API does not blacklist subdomains nor legitimate domains, while Content scan works only if link is an actual website and contains html content. Because the nature of direct download, there are no content for "Content scan" to scan.&#x20;

Example link of how these criminals take advantage of legitimate website service

mediafire.com/abcdef\
github.com/something.exe\
\
\
This is where URL List comes in, to cover these type of issues. The URL List are scanned and vetted by Munio's staff and if they deem a specific URL to be malicious, it will be blacklisted. However, unlike the scanner type "Blacklist", URL list does NOT ban the actual domain. Instead it bans the specific URL string instead.&#x20;

If bot blacklist github.com/something.exe\
then github.com will not be blacklisted.

## Default: <mark style="color:green;">Enabled</mark>

Bot will by default delete message and timeout users from all servers if the user post a detected link from Munio internal database.&#x20;

**Default punishment type**: Delete & Timeout

\
To configurate this scanner, follow these steps:

> **/punishment set-punishment scanner:URL List**
