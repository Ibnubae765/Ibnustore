<p align="center">
<img src="https://readme-typing-svg.herokuapp.com?color=%2336BCF7&center=true&vCenter=true&lines=S+C+R+I+P+T+ㅤ+B+Y+ㅤ+ID+S+T+O+R+E" />
</p>
#!/bin/bash

# Warna hijau
GREEN='\033[0;32m'
# Reset warna
NC='\033[0m'

# Teks yang akan dianimasikan
TEXT="AUTOSCRIPT BY ID STORE"

# Fungsi untuk menampilkan teks dengan animasi bergerak
animate_text() {
    local length=${#TEXT}
    while true; do
        for (( i=0; i<length; i++ )); do
            clear
            echo -e "${GREEN}${TEXT:0:i}${NC}"
            sleep 0.1
        done

        for (( i=length; i>0; i-- )); do
            clear
            echo -e "${GREEN}${TEXT:0:i}${NC}"
            sleep 0.1
        done
    done
}

# Panggil fungsi animasi
animate_text
