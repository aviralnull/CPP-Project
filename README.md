End To End Encrypted Chat Server 

# Compile Client file to object file
g++ -c tls_client_p.cpp -o tls_client_p.o -I C:/path_to_openssl/include

# Link object file to create executable
g++ tls_client_p.o -o tls_client_p.exe \
    -L"C:/msys64/mingw64/bin" \
    -L"C:/Users/harsh/Downloads/boost_1_88_0/boost_1_88_0/stage/lib" \
    -lssl -lcrypto -lws2_32 -lwsock32 \
    -lboost_system-mgw15-mt-x64-1_88

   # Compile Server file to object file 
g++ -c tls_server_p.cpp -o tls_server_p.o -I C:/path_to_openssl/include 

# Link object file to create executable
 g++ tls_server_p.o  -o tls_server_p.exe `   
>>   -L"C:/msys64/mingw64/bin" `                                                                                                                 
>>   -L"C:/Users/harsh/Downloads/boost_1_88_0/boost_1_88_0/stage/lib" `
>>   -lssl -lcrypto -lws2_32 -lwsock32 `
>>   -lboost_system-mgw15-mt-x64-1_88
>> 

#These are based on my file paths  update this accordingly 
