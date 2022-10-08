#Create a database
Database_Name: `api`
--------------------------------------------------------------------------------------
#Table structure for table `users`

CREATE TABLE `users` (
  `id` int(11) NOT NULL,
  `username` varchar(255) NOT NULL,
  `password` varchar(255) NOT NULL,
  `created` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
--------------------------------------------------------------------------------------
#Add primary key to 'id'

ALTER TABLE `users`
  ADD PRIMARY KEY (`id`);
--------------------------------------------------------------------------------------
#Add auto_increment to 'id'

ALTER TABLE `users`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=2;
COMMIT;
--------------------------------------------------------------------------------------

Credit :- Deepraj Pagares
