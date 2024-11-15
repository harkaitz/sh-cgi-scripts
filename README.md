CGI SCRIPTS
===========

Shell and python scripts for writting small CGI WEB programs.

## Help

cgiw

    Usage: cgiw COMMAND
    
    Execute command, if it fails print a CGI HTTP 400 error response.

html_body

    Usage: html_body < HTML_BODY > HTML 
           html_body -c COMMAND  > HTML
    
    Place the input or the command's output between <html><body>...</body></html>.

httpd_pycgi

    Usage: httpd_pycgi [-p PORT (default 8080)] DIRECTORY
    
    Serve directory with a HTTP server using python's http.server
    module. You should name CGI scripts as "DIRECTORY/cgi-bin/NAME"
    and make them executable.

md2html

    Usage: md2html < MARKDOWN > HTML_BODY
           md2html -c COMMAND > HTML_BODY
    
    Convert markdowns to html using python (pip3 install markdown).

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
