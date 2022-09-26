ejerciocio 1
INSERT INTO `store` (`ID`, `PROFILE`, `NAME`, `LAT`, `LNG`, `IdRubro`) VALUES
(8, 1, 'atm', -37.9987, -57.5526, 0),
(2, 1, 'Banco Nacion de la Argentina', -37.9997, -57.5468, 1),
(3, 1, 'Banco Provincia', -37.9993, -57.5465, 1),
(4, 0, 'Astor', -38.0008, -57, 2),
(5, 0, 'Musical Norte', -37.9993, -57.5484, 3),
(1236711896, 0, 'Musical Norte', -37.9993, -57.5484, 3),
(285071699, 0, 'Astor', -38.0008, -57, 1),
(1236940209, 0, 'atm', -37.9987, -57.5526, 0),
(288366501, 1, 'Banco Nacion de la Argentina', -37.9997, -57.5468, 1),
(1236707570, 1, 'Banco Provincia', -37.9993, -57.5465, 1);
COMMIT;

ejerciocio 2

ejerciocio a
SELECT * FROM STORE WHERE ID > 100 && ID < 2500;

ejerciocio b
SELECT * FROM STORE WHERE PROFILE >= 1 && PROFILE <=3 && ID>10000;

ejerciocio c
SELECT * FROM STORE WHERE (IdRubro = 1 || IdRubro = 2 )&& LOCATE("Banco",NAME)>0;

ejerciocio d
SELECT MAX(ID),NAME FROM STORE;

ejerciocio e
SELECT MIN(LAT),NAME FROM STORE;

ejerciocio 3

ejerciocio a
UPDATE STORE SET NAME = "Banco Nacion de la Argentina" WHERE NAME = "Banco Nacion";


ejerciocio b
UPDATE STORE SET NAME = "Musical Norte" WHERE NAME = "AGB";


ejerciocio c
UPDATE STORE SET LNG = -57.000001 WHERE NAME = "Astor";