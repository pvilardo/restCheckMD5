# restCheckMD5
In my short experience using REST JSON call, I used to manage big data list and  waiting seconds to receive the same response
I get tired and create this project.9)
The idea is simple, when you receive a big data reponse from a REST Endpoint you also receive a MD5 Checksum (MD5-DataCheck:<MD5String>) (like Content-MD5) but the purpose 
is to sent it back to the endpoint, if the MD5 matches, the response will return empty, with the headers,  MD5 check and a flag (MD5-DataEquals:true).
This project is useless for reactive protocols, like WebSocket or HTTP event stream frameworks (Spring Flux, or else), because 
those project sent the deltas/updates/etc after you connect (and subscribe if needed).




