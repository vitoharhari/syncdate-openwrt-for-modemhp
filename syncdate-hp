#!/bin/bash
adb shell date
adb shell date > /root/hasildate

hari=$(cat /root/hasildate | cut -b 9-10)
bulan=$(cat /root/hasildate | cut -b 5-7)
tahun=$(cat /root/hasildate | cut -b 25-28)
waktu=$(cat /root/hasildate | cut -b 12-19)

    case $bulan in
        "Jan")
            bulan="01"
            ;;
        "Feb")
            bulan="02"
            ;;
        "Mar")
            bulan="03"
            ;;
        "Apr")
            bulan="04"
            ;;
        "May")
            bulan="05"
            ;;
        "Jun")
            bulan="06"
            ;;
        "Jul")
            bulan="07"
            ;;
        "Aug")
            bulan="08"
            ;;
        "Sep")
            bulan="09"
            ;;
        "Oct")
            bulan="10"
            ;;
        "Nov")
            bulan="11"
            ;;
        "Dec")
            bulan="12"
            ;;
        *)
            continue
    esac
    
    case $hari in
        " 1")
            hari="01"
            ;;
        " 2")
            hari="02"
            ;;
        " 3")
            hari="03"
            ;;
        " 4")
            hari="04"
            ;;
        " 5")
            hari="05"
            ;;
        " 6")
            hari="06"
            ;;
        " 7")
            hari="07"
            ;;
        " 8")
            hari="08"
            ;;
        " 9")
            hari="09"
            ;;
        *)
            continue
    esac


date -s $tahun.$bulan.$hari-$waktu
