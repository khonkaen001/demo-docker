
// สร้างไฟล์ Dockerfile ก่อน

FROM [ตัวรัน server เช่น nginx]:latest [version]

COPY ./index.html /usr/share/nginx/html/index.html

COPY [ไฟล์] [pattern การนำไฟล์ขึ้น]/[ชื่อไฟล์ที่จำนำขึ้น]

คำสั่ง Docker 

// สร้าง docker-image โดยการ Build ทุกครั้งที่แก้ต้อง build ใหม่
docker build -t demo_image . 

docker build -t [ชื่อDockerImage] . 

//run Docker
    
docker run -p 8081:80 demo_image

docker run -p [port]:80 [imageName]