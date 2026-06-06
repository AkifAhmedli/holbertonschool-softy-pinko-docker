# 1. Ən son Ubuntu obrazından istifadə edirik
FROM ubuntu:latest

# 2. APT paket menecerini yeniləyirik
RUN apt-get update

# 3. Mövcud proqram təminatlarını təkmilləşdiririk (-y avtomatik təsdiq üçündür)
RUN apt-get upgrade -y

# 4. Konteyner işə düşəndə ekrana "Hello, World!" yazdırırıq
CMD ["echo", "Hello, World!"]
