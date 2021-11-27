# Jarkom-Modul-4-A05-2021

Kelompok A5 :
<li>05111840000138 - Gema Adi Perwira
<li>05111940000024 - Hanifa Fauziah
<li>05111940000111 - Evelyn Sierra
  
 ## Topologi
 ![image](https://user-images.githubusercontent.com/55088939/143670280-f9547f1d-e5b8-4ed6-93af-927abae9c3c8.png)

 ## CPT - VLSM
  ### Pembagian Subnet
  ![image](https://user-images.githubusercontent.com/55088939/143670299-896f94ed-9fc1-4ccd-9d6d-7d3919730ec5.png)

  ### Perhitungan subnet
  ![image](https://user-images.githubusercontent.com/55088939/143670325-714c5d92-fbd9-436b-a3aa-d255bf6bb7a9.png)

  ### VLSM Tree
  ![image](https://user-images.githubusercontent.com/55088939/143670394-75b02a9a-43a7-4c94-8ca8-6401efb82f06.png)

  ### Pembagian IP
  ![image](https://user-images.githubusercontent.com/55088939/143670342-2267dc07-27b3-4ccc-aac3-2667f20b02d1.png)

  ### Routing
  #### Subnet A8
  
  Pada **Foosha** ke Blueno
  ```
ipv4 address 192.171.16.1
netmask 255.255.252.0
```
Pada **Blueno** ke Foosha
  ```
ipv4 address 192.171.16.2
netmask 255.255.252.0
gateway 192.171.16.1
  ```
  
  #### Subnet A5
  
  Pada **Foosha** ke Water7
  ```
ipv4 address 192.171.0.5
netmask 255.255.255.252
```
Pada **Water7** ke Foosha
  ```
ipv4 address 192.171.0.6
netmask 255.255.255.252
  ```
  Default Routing pada **Water7**
  ```
ip network 0.0.0.0
mask 0.0.0.0
next hop 192.171.0.5
  ```
  
  #### Subnet A4
  Pada **Water7** ke Cipher
  ```
ipv4 address 192.171.8.1
netmask 255.255.252.0
  ```
  Pada **Cipher** ke Water7
  ```
ipv4 address 192.171.8.2
netmask 255.255.252.0
gateway 192.171.8.1
```
  Pada **Foosha** Static
  ```
ip network 192.171.8.0
mask 255.255.252.0
nexthop 192.171.0.6
  ```
  
#### Subnet A3
  Pada **Water7** ke Pucci
  ```
ipv4 address 192.171.0.1
netmask 255.255.255.252
```
Pada **Pucci** ke Water7
```
ipv4 address 192.171.0.2
netmask 255.255.255.252
  ```
  Default Routing pada **Water7**
  ```
ip network 0.0.0.0
mask 0.0.0.0
next hop 192.171.0.1
```
 Pada **Foosha** Static
  ```
ip network 192.171.0.0
mask 255.255.255.252
nexthop 192.171.0.6
  ```
  
#### Subnet A1
  Pada **Pucci** ke Jipangu
  ```
ipv4 address 192.171.0.129
netmask 255.255.255.128
```
Pada **Jipangu** ke Pucci
  ```
ipv4 address 192.171.0.130
netmask 255.255.255.128
gateway 192.171.0.129
```
Pada **Water7** Static
  ```
ip network 192.171.0.128
mask 255.255.255.128
nexthop 192.171.0.2
```
Pada **Foosha** Static
```
ip network 192.171.0.128
mask 255.255.255.128
nexthop 192.171.0.6
 ```
  
#### Subnet A2
  
  
  
  
  
 ## GNS3 - CIDR
  
  ### Pembagian subnet
  Langkah 1
  ![image](https://user-images.githubusercontent.com/55088939/143670551-33a69414-d7ea-433d-853c-e9479aa1c24f.png)
  
  Langkah 2
  ![image](https://user-images.githubusercontent.com/55088939/143670574-941bc620-42f1-4a7c-baa4-780c2452afb2.png)

  Langkah 3
  ![image](https://user-images.githubusercontent.com/55088939/143670579-904cdfd7-20af-4578-aae3-005582e6b30c.png)

  Langkah 4
  ![image](https://user-images.githubusercontent.com/55088939/143670586-55b61728-833e-4d9c-bb2e-2efa19b32bb2.png)

  Langkah 5
  ![image](https://user-images.githubusercontent.com/55088939/143670594-bfeb6363-95e5-4dcb-b00a-50494de1c6b9.png)

  Langkah 6
  ![image](https://user-images.githubusercontent.com/55088939/143670599-5f5e4499-f47e-4370-82fd-6e81ed4787cd.png)

  Langkah 7
  ![image](https://user-images.githubusercontent.com/55088939/143670661-6fc72859-443d-4789-9c4a-aa2816719c13.png)

  ### CIDR Tree
  ![image](https://user-images.githubusercontent.com/55088939/143670669-3b419a0f-6484-42b8-9a5d-8d5ab78771b5.png)

  ### Setting GNS3
  
  ### Routing
  
 ## Kendala
  
