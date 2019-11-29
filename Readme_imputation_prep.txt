
#Connec to server
sftp tenghe@10.162.228.2 #Usually to collect data or submit jobs

#Change Marker name in Reference Genome VCF files
bcftools annotate --set-id +'%CHROM\_%POS' Chr25.vep.vcf.gz | bgzip > test25.vcf.gz

#Add an executable to $PATH to permit global execution without specifying $PATH
sudo cp Minimac3 /usr/local/bin
Minimac3

#Run beagle
java -jar beagle.28Sep18.793.jar

