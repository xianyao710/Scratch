#fastq converted to fasta

sed -n -e '1~4s/^@/>/p;2~4p' $1 .fastq > .fasta
