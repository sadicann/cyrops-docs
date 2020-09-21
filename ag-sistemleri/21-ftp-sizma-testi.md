# 21/FTP Sızma Testi

## Temel Bilgiler

Açılımı **File Transfer Protocol** olan FTP’nin Türkçe karşılığı **Dosya Transfer Protokolü**’dür. İsminden de anlaşılabileceği gibi internete bağlı iki bilgisayar arasında dosya transferini sağlayan bir protokol ve bu işleme hizmet eden uygulamaya verilen isimdir. Örneğin bir web sitende yer alması istenen dosyalar sunuculara FTP üzerinden aktarılabilir.

**Varsayılan Port:** 21/TCP

## Keşif

### FTP Port Tespiti

Sunucuda FTP servisinin tespiti için NMAP ile servis taraması yapılır.

```text
nmap -sV -T4 -O -F 192.168.1.1
```

 FTP servisinin aktif olması durumunda aşağıdaki gibi STATE/open ve SERVICE/ftp çıktısı alınacaktır.

```text
PORT   STATE SERVICE
21/tcp open  ftp
```



