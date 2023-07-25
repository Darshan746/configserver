
for encrypting the property in the config-server

first we have to decalre the property name called
encrypt.key=eazybytes
the value of the above property could be anything which you want ,this value would be used while encrypting
and decrypting the value

first we have to get the encrypted value of the property which you want to encrypt
and have it in the config server application.properties file prefix with {cipher}
here in this example have a look at application.properties file here


you have to trigger the 2 POST Request end points in the config server for encryption and decryption

1] to get the actual value of the encrypted value

     <HOST>:<PORT>/decrypt

    it should be post request with the body 
the body should be of the text which contains the encrypted value


2] to get the  encrypted value

    <HOST>:<PORT>/encrypt

    it should be post request with the body 
the body should be of the text which contains the actual  value to be decrypt