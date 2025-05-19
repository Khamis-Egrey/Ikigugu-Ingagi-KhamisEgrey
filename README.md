<?php
$backupFile = 'backup_' . date("Y-m-d_H-i-s") . '.sql';
$command = "mysqldump --user=root ingagi_db > $backupFile";
system($command, $output);
echo "Database backup completed: $backupFile";
?>
