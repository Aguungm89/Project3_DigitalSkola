# Project3_DigitalSkola
# Project Batch Processing

Case:
Description
Tugas kalian adalah mengolah data covid-19 di Jawa Barat dari raw data sampai ke
data warehouse dalam bentuk star schema. Data yang di dapat adalah data kasus
harian per kabupaten/kota. Data yang dibutuhkan adalah data agregat dalam jangka
waktu tertentu per kabupaten/kota dan per provinsi.

Notes
1. Use every knowledge from previous learning session
2. Use OOP for code structure
3. Load credential for databases from file, make sure no secrets are shown in code

Project Steps
1. Create DDL in MySQL
2. Get data from Public API covid19 and load data to MySQL
3. Create DDL in PostgreSQL for Fact table and Dimension table
4. Create aggregate Province Daily save to Province Aggregate Table
5. Create aggregate Province Monthly save to Province Aggregate Table
6. Create aggregate Province Yearly save to Province Aggregate Table
7. Create aggregate District Daily save to District Aggregate Table
8. Create aggregate District Monthly save to District Aggregate Table
9. Create aggregate District Yearly save to District Aggregate Table

Table Specification
Dimension table
1. Province table
  a. province_id
  b. Province_name
2. District table
  a. district_id
  b. province_id
  c. district_name
3. Case table
  a. id (auto generate)
  b. status_name (suspect, closecontact, probable, confirmation)
  c. status_detail

Fact table

1. Province Aggregate Table
  a. Id (auto generate)
  b. province_id
  c. case_id
  d. date
  e. Total
2. District Aggregate Table
  a. Id (auto generate)
  b. district_id
  c. case_id
  d. month
  e. total




