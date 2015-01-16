README
This is based on a code sample provided at https://github.com/alcazes/PHP-REST-REPORTING-API but alters it in two ways:
1.  It is adapted to run on the command line rather than in a web browser.
2.  It has a very basic "index.php" file that is executed to call the function and return data.

You will need PHP installed and the php_curl.dll library added to the php.ini configuration file.

To configure the script, open the reportRankedRest.php file and search for square brackets "[".  This will show all credentials and configuration options to be set.  You can remove the proxy related cURL options if you connect directly to the internet, just delete the CURLOPT_PROXY lines from reportRankedRest.php.

To run the script, call php.exe from the Windows command prompt with the path to index.php added e.g. php.exe 
"c:\script\index.php".  It should return a table of data for the top 25 pages in your report suite and the view count.

This is provided without warranty of any kind.