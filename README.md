# CNVpytorVCF
CNVpytor plugin for JBrowse


## Installation
JBrowse dev version installation
```
# Jbrowse Git: https://github.com/GMOD/jbrowse/releases

# Download JBrowse 1.16.8
wget https://github.com/GMOD/jbrowse/archive/1.16.8-release.tar.gz
# Extract
tar xzf 1.16.8-release.tar.gz
# Rename
mv jbrowse-1.16.8-release jbrowse
```
**Plugin install:** To install a JBrowse plugin, copy the plugin in the JBrowse plugin directory 


```
cd plugins
git clone https://github.com/arpanda/CNVpytorCNV.git
```
Dependencies
 
To Install [ml-levenberg-marquardt](https://www.npmjs.com/package/ml-levenberg-marquardt), use by the following command in the JBrowse root directory
```batch
yarn add ml-levenberg-marquardt
```

 #### load plugin on localhost
 ```
 http://localhost/jbrowse/?data=plugins/CNVpytorCNV/test/data
 http://localhost/jbrowse/?data=test_vcfview