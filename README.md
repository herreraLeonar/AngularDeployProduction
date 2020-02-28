# deploy production angular 8. Express NodeJS

working with aws t2.small ubuntu 18.04
pm2, apache2

angular project

For prod build, run following command:

create swap

# free -h

# sudo /bin/dd if=/dev/zero of=/var/swap.1 bs=1M count=8196

# sudo /sbin/mkswap /var/swap.1

# sudo chmod 600 /var/swap.1

# sudo /sbin/swapon /var/swap.1

# sudo swapon --show

To enable it by default after reboot, add this line to /etc/fstab:
# /var/swap.1 swap swap defaults 0 0

restart instance aws

# set NODE_OPTIONS=--max-old-space-size=4096

# node --max_old_space_size=4096 ./node_modules/.bin/ng build --prod


# cd ../AngularDeployProduction

# pm2 start index.js
