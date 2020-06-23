# wsdls

## Configure

    Step number 1
        Cree un host virtual para una carpeta wsdl y dentro incluya el archivo soapServer.wsdl
            Example:
                <VirtualHost *:80>
                    DocumentRoot "/opt/lampp/htdocs/wsdl"
                    ServerName wsdl.doc

                    ErrorLog "logs/wsdl.doc-error_log"
                    CustomLog "logs/wsdl.doc-access_log" common
                </VirtualHost>

    Step number 2
        In the /etc/hots file add the ServerName of the VirtualHost previously created and restart the server
            Example: 
                127.0.0.1	wsdl.doc
