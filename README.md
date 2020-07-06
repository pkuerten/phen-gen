# phen-gen

We introduce Phen-Gen, a method that combines patients' disease symptoms and sequencing data with prior domain knowledge to identify the causative genes for rare disorders. Simulations revealed that the causal variant was ranked first in 88% of cases when it was a coding variant—a 52% advantage over a genotype-only approach—and Phen-Gen outperformed other existing prediction methods by 13–58%. If disease etiology was unknown, the causal variant was assigned the top rank in 71% of simulations. Phen-Gen is available at http://phen-gen.org/.

![Overview](/figure1overview.png)

# Citation
Javed, A., Agrawal, S. & Ng, P. C. Phen-Gen: combining phenotype and genotype to analyze rare disorders. Nat Methods. 2014 Sep;11(9):935-7. doi:10.1038/nmeth.3046. Epub 2014 Aug 3. PubMed PMID: 25086502.

# Phen-Gen standalone

Our standalone (Version 1.0) is available under the GNU General Public License. It has been tested in Linux environment (Ubuntu 12.04.3 LTS, CentOS 6.1, and RHEL 6.1).

To install the standalone:
Check that Perl is already installed: type perl -v on the command line. If it's not available, click here to install it.
Download the standalone(https://www.dropbox.com/s/5go2pvzer46e0g9/Phen-GenV1.tar.gz?dl=0). (Size 2.9 GB)
Transfer the downloaded file to the directory where you want to run it (e.g. /home/yourusername/phengen).
To decompress and extract the contents of the standalone: tar -zxvf Phen-GenV1.tar.gz
To run the standalone:

Execute the command:
perl phen-gen.pl input_phenotype=< text > input_vcf=< vcf > input_ped=< ped > inheritance=< i > predictor=< p > stringency=< s > discard_de_novo=< d > 

Please refer to README.txt for a description of the command line and its parameters, and file formats. The approximate run time is 15 minutes. 
