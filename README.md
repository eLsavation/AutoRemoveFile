# autoremovefile

auto remove file in 3 day

apt install git clone

git clone https://github.com/eLsavation/autoremovefile.git

cd autoremovefile

vim remove3d.sh 

#customize the path or file you want to delete

crontab -e 

#add 0 1 * * * /path/autoremovefile/remove3d.sh 

done
