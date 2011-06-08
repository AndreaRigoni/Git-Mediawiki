#Sandbox for further developing

[Last status mail](http://www.spinics.net/lists/git/msg158701.html)

## Partial clones
Nobody wants to clone wikipedia entirely. We would like to add a list of pages that one would want to track and only fetch revisions from these pages. 

### Possibility to add more pages overtime
One would like to track other pages. We need to create a command to add these pages to the repository.
Issue : Necessity to rewrite the entire history

## Possibility to log in to the wiki
The mediawiki->login method from the API returns a sessionid. If we cross it with mediawiki->{ua}->{cookie_jar}, it should be able to maintain session between two calls without having to re-login. To go further, it could be really nice to type something in the lines of "git config remote.$remotename.username" to get the username pretending it is stored in .git/config and use Term::ReadKey; ReadMode('noecho'); $password = ReadLine(0); to get the password

## Clone tracked pages
Combining Partial clones and login possibilities, it could be also nice to login and only clone pages that are tracked by a user.

## Merge patterns
See mail

## Sending attached files to wiki pages
In mediawiki one can upload and download images, videos, archives, etc to wiki pages. The Mediawiki enbales that thanks to [Mediawiki::API->dowload($params_hash)](http://search.cpan.org/~exobuzz/MediaWiki-API-0.24/lib/MediaWiki/API.pm#MediaWiki::API-%3Eupload%28_$params_hash_%29) and [Mediawiki::API->download($params_hash)](http://search.cpan.org/~exobuzz/MediaWiki-API-0.24/lib/MediaWiki/API.pm#MediaWiki::API-%3Edownload%28_$params_hash_%29).



###