server {
   listen 80;
   listen [::]:80;
   server_name flowhealth.duckdns.org; # CHANGE SERVER NAME TO YOUR REGISTERED DOMAIN

   location / {
         proxy_pass http://localhost:8099; # CHANGE PORT TO YOUR UNIQUE PORT
         # Simple requests
         if ($request_method ~* "(GET|POST)") { # Customize Request methods based on your needs
                  add_header "Access-Control-Allow-Origin"  *;
         }

         # Preflighted requests
         if ($request_method = OPTIONS ) {
                  add_header "Access-Control-Allow-Origin"  *;
                  add_header "Access-Control-Allow-Methods" "GET, POST, OPTIONS, HEAD";
                  add_header "Access-Control-Allow-Headers" "Authorization, Origin, X-Requested-With, Content-Type, Accept";
                  return 200;
          }

    }

}