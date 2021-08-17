# debian-tut - how to trigger debian packaging process for hello01 and hello02     
cd hello01   
tar -zcvf yockgen01-0.1.tar.gz ./yockgen01-0.1/    
cd yockgen01-0.1/    
debmake   
debuild -us -uc   
