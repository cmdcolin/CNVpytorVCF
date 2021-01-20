# CNVpytorVCF
CNVpytor plugin for JBrowse


## Demo example for CNVpytor export and CNVpytorVCF plugin
Demo page with Hg19 reference: https://abyzovlab.github.io/CNVpytorVCF/JBrowse/
#### CNVpytor export
Read depth and BAF analysis is done for HepG2 genome using CNVpytor and both BAM and VCF file are used here. Three different bin sizes (i.e.; 1K, 10K, 100K) are used for detailed understanding. JBrowse page automatically selects the bin size based on the length of the selected region.
#### CNVpytorVCF plugin
Demo example takes the HepG2 vcf file, which supplied together with this plugin. Currently, it takes 100k as bin size.
Plugin does on the fly calculation for read depth and BAF analysis. A new vcf file can be loaded using the tools menu. 





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
