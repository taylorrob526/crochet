# crochet
An inventory of crochet projects and patterns

CREATE TABLE crochet_store (id INTEGER PRIMARY KEY, name TEXT, category TEXT, price INTEGER, quantity INTEGER, pattern TEXT); 

INSERT INTO crochet_store VALUES (1, "Striped Hat", "clothing", 8.99, 10, "yes");
INSERT INTO crochet_store VALUES (2, "Cozy Knit Scarf", "clothing", 12.99, 15, "yes");
INSERT INTO crochet_store VALUES (3, "Sleek Black Wallet", "accessories", 30.00, 25, "yes");
INSERT INTO crochet_store VALUES (4, "Baby Hat with Pom Pom", "clothing", 5.99, 20, "yes");
INSERT INTO crochet_store VALUES (5, "Children's Hat with Pom Pom", "clothing", 6.99, 20, "yes");
INSERT INTO crochet_store VALUES (6, "Adult Beanie", "clothing", 8.99, 30.00, "yes");
INSERT INTO crochet_store VALUES (7, "Brown Crossbody Bag", "accesories", 45.99, 10, "no");
INSERT INTO crochet_store VALUES (8, "0-3 months babydoll dress", "clothing", 15.99, 5, "no");
INSERT INTO crochet_store VALUES (9, "4-6 months dress", "clothing", 16.99, 10, "no");
INSERT INTO crochet_store VALUES (10, "7-9 months dress", "clothing", 16.99, 5, "no");
INSERT INTO crochet_store VALUES (11, "9-12 months dress", "clothing", 17.99, 10, "yes");
INSERT INTO crochet_store VALUES (12, "Diamond Baby Blanket", "home", 60.00, 3, "yes");
INSERT INTO crochet_store VALUES (13, "Bunny Amigurumi", "toys", 9.99, 15, "yes");
INSERT INTO crochet_store VALUES (14, "Pokemon: Squirtle", "toys", 25.99, 10, "no");
INSERT INTO crochet_store VALUES (15, "Summer Breeze Sundress", "clothing", 35.99, 10, "yes");
INSERT INTO crochet_store VALUES (16, "Pokemon: Vaporeon", "toys", 25.99, 10, "no");

SELECT * FROM crochet_store GROUP BY category ORDER BY price;

SELECT SUM(quantity) FROM crochet_store GROUP BY category;

SELECT name, price FROM crochet_store ORDER BY price

