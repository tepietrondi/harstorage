sudo python setup.py bdist_egg
sudo easy_install-2.7 dist/harstorage-1.0-py2.7.egg

phantomjs examples/netsniff.js http://www.domain.com > www.domain.com.har 

curl --verbose --header "Automated: true" --form "file=@www.domain.com.har " http://localhost:5000/results/upload
