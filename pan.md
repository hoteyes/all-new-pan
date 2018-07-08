when HTTP_REQUEST {
 if { [HTTP::host] equals "test.example.com" } {
   HTTP::redirect "https://test.example.com/idp/startSSO.ping?"
} else {
   pool WEB_HTTP_POOL1
   } 
}