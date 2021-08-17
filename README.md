# debian-tut - how to trigger debian packaging process for hello01 and hello02     

**Step 1: create tarball for source code**      
cd hello01      
tar -zcvf yockgen01-0.1.tar.gz ./yockgen01-0.1/    

**Step 2: building debian package**       
cd yockgen01-0.1/    
debmake   
debuild -us -uc  

**Step 3: test debian package**              
sudo dpkg -i yockgen01_0.1-1_amd64.deb     
ls /usr/bin/yockgen01   
sudo dpkg -P yockgen01   

