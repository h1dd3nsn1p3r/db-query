#### ✅ CREATE

    CREATE TABLE `Class_C` (
    `id` int(11) NOT NULL AUTO_INCREMENT,
    `name` varchar(255) NOT NULL,
    `age` int(10) NOT NULL,
    PRIMARY KEY (`id`)
    );


#### ✅ INSERT

    INSERT INTO `Class_C` (`name`, `age`) VALUES ('Anuj Subedi', 29);

  
#### ✅ SELECT

    SELECT * FROM `Class_C`;
    
    SELECT * FROM `Class_C` WHERE `id` = 1;


#### ✅ DELETE

    DELETE FROM `Class_C` WHERE `id` = 1;
    
    DELETE FROM `Class_C` WHERE `name` = 'Anuj Subedi';


#### ✅ UPDATE

    UPDATE `Class_C` SET name='John' WHERE id=2;

  
#### ✅ ALTER

    ALTER TABLE `Class_C` ADD `address` VARCHAR(255) NOT NULL AFTER `age`;
    
    ALTER TABLE `Class_C` DROP `address`;
    
    ALTER TABLE `Class_C` CHANGE `name`  `Fname` VARCHAR(255) NOT NULL;
    
    ALTER TABLE `Class_C` MODIFY `name` VARCHAR(255) NOT NULL;
    
    ALTER TABLE `Class_C` RENAME TO `Class_D`;

#### ✅ DROP

    DROP TABLE `Class_C`;
    
    DROP TABLE IF EXISTS `Class_C`;

  
#### ✅ TRUNCATE

    TRUNCATE TABLE `Class_C`;


#### ✅ IMPORT DATABASE

    mysqldump -uUSERNAME -p DATABASE_NAME > backup.sql


#### ✅ EXPORT DATABASE

    mysql -uUSERNAME -p DATABASE_NAME < backup.sql
