# Attendance
Attendance System
`user` (
  `id` int NOT NULL AUTO_INCREMENT,
  `fullname` text NOT NULL,
  `email` text NOT NULL,
  `role` text NOT NULL,
  `class` text NOT NULL,
  PRIMARY KEY (id)
);

CREATE TABLE `class` (
  `id` int NOT NULL AUTO_INCREMENT,
  `name` text NOT NULL,
	PRIMARY KEY (id),
   UNIQUE KEY (name(255))
);

CREATE TABLE `attendance` (
  `studentid` int NOT NULL,
  `classid` int NOT NULL,
  `session` int NOT NULL,
  `ispresent` int NOT NULL
);
