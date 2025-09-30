##### read index.php : 

it accept just zip files
we can see our uploaded files
it accept just .txt .jpg files ( ziped files ) to access them 

we will create the amazing that file : 

ln -s ../../../index.php index.txt
zip --symlinks index.zip index.txt


upload it , and bom 

---
why it happend :  **Unsafe decompression**

when we upload the zip file , he still pointed to ../../../index.php , and the server is no secure , and it accept it and follow the path we specified , bom .