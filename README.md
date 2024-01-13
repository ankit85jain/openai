Table orders {
  id int [primary key]
  user_id int [not null, unique]
  status varchar
  created_at varchar
}

Table order_items  {
  order_id int
  product_id int
  quantity int
}

Table products  {
  id int [primary key]
  name varchar
  merchant_id int [not null]
  price int
  status varchar
  created_at varchar
  category_id int
}

Table users {
  id int [primary key]
  full_name varchar
  email varchar [unique]
  gender varchar
  date_of_birth varchar
  created_at varchar
  country_code int
}
