create table menu (
    item_id int primary key auto_increment,
    item	varchar(255),
    description varchar(1024),
    item_type varchar(15), check (item_type in ('Tapas', 'Drinks', 'Entries', 'Sides', 'Dessert')),
    price float,
    start_date date,
    end_date date) ;
    
    item_id int primary key auto_increment,
    "Fried Pickles"	varchar(255),
    'Shareable basket of golden-fried pickle chips served with Ranch or Cajun sauce for dipping' varchar(1024),
    'Tapas' varchar(15), check (item_type in ('Tapas', 'Drinks', 'Entries', 'Sides', 'Dessert')),
    7.49 float,
    '2019-04-21' date,
    '2025-12-31' date) ;
    
    item_id int primary key auto_increment,
    'Sweet Potato'	varchar(255),
    '' varchar(1024),
    'Sides' varchar(15), check (item_type in ('Tapas', 'Drinks', 'Entries', 'Sides', 'Dessert')),
    3.49 float,
    '2019-04-21' date,
    '2025-12-31' date) ;
    
     item_id int primary key auto_increment,
    'Hand-Cut Sirloin 16Oz'	varchar(255),
    'Lean, juicy steak priced at a great value. Served with choice of two sides.' varchar(1024),
    'Entries' varchar(15), check (item_type in ('Tapas', 'Drinks', 'Entries', 'Sides', 'Dessert')),
    26.99 float,
    '2019-04-21' date,
    '2025-12-31' date) ;
    
    item_id int primary key auto_increment,
    'Strawberry Cheesecake'	varchar(255),
    'Slice of classic New York-style cheesecake topped with strawberry sauce and whipped cream' varchar(1024),
    'Desert' varchar(15), check (item_type in ('Tapas', 'Drinks', 'Entries', 'Sides', 'Dessert')),
    7.99 float,
    '2019-04-21' date,
    '2025-12-31' date) ;
    
    item_id int primary key auto_increment,
    'Fountain Drink'	varchar(255),
    '' varchar(1024),
    'Drinks' varchar(15), check (item_type in ('Tapas', 'Drinks', 'Entries', 'Sides', 'Dessert')),
    2.49 float,
    '2019-04-21' date,
    '2025-12-31' date) ;
 
 SELECT * FROM menu ;
 update menu set item='Fountain Drinks' where item_id = 5 ;
