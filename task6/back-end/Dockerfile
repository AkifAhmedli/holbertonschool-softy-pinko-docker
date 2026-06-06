# 1. Ən son Ubuntu əsaslı imic
FROM ubuntu:latest

# 2. APT sistemini yeniləyirik
RUN apt-get update

# 3. Mövcud proqramları yeniləyirik
RUN apt-get upgrade -y

# 4. Python3 və Pip3 quraşdırırıq
RUN apt-get install -y python3 python3-pip

# 5. Pip xətasının (Externally Managed Environment) qarşısını almaq üçün bu sətiri mütləq əlavə edirik
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# 6. Pip3 vasitəsilə flask quraşdırırıq
RUN pip3 install flask

# 7. Konteyner daxilində işçi qovluğu /app təyin edirik
WORKDIR /app

# 8. api.py faylını kompüterdən konteynerin daxilinə (/app/api.py kimi) kopyalayırıq
COPY ./api.py /app/api.py

# 9. Konteyner işə düşəndə Flask serverini başladırıq
CMD ["python3", "api.py"]
