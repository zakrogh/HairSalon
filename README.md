CREATE SCHEMA `zach_krogh` ;

CREATE TABLE `stylists` (
  `stylistid` serial,
  `name` varchar(255) NULL,
  `specialty` varchar(255) NULL,
  PRIMARY KEY (`stylistid`));

CREATE TABLE `zach_krogh`.`clients` (
  `clientid` serial,
  `name` VARCHAR(255) NULL,
  `stylistid` INT(11) NULL,
  PRIMARY KEY (`clientid`));
