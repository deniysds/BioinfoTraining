
# Genomic Bioinformatics Crash Course
Pelatihan ini ditujukan untuk dapat memberikan pemahaman dasar untuk pengolahan informasi bioinformatik yang dari proses sekuensing. Penyusunan pelatihan ini dilakukan agar setiap peneliti dan institusi penelitiannya dapat menyusun sumber daya secara mandiri mulai dari menyusun komputer yang sesuai sampai melakukan analis.

##  Persiapan Cloud
### 1. Instance CPU Based
####  Minimum Requirenment
- Operating System : Ubuntu 22.04
- RAM : 16GB
- CPU : 4 Core

#### Software Pendukung Sequencing
1. SRAtoolkit : https://github.com/ncbi/sra-tools/wiki/01.-Downloading-SRA-Toolkit
2. Trimometric : http://www.usadellab.org/cms/uploads/supplementary/Trimmomatic/Trimmomatic-0.39.zip
3. BWA mem : https://github.com/lh3/bwa/releases/tag/v0.7.17
4. GATK : https://github.com/broadinstitute/gatk/releases
5. Samtools : https://github.com/samtools/samtools/releases
6. BCFtools : http://www.htslib.org/download/
7. Picard : https://github.com/broadinstitute/picard/releases
8. Telomere to Telomere : https://github.com/marbl/CHM13

#### Petunjuk Login ke Terminal
> Login via username dan password :
ssh [username]@[ip_address]
`$ ssh root@110.239.66.155`

> Login with keypair
ssh -i [key_file] [username]@[ip_address]
>- same path
`$ ssh -i training_bioinfo_peserta.pem root@110.239.69.17`
> - diferent path
`$ ssh -i /opt/training_bioinfo_peserta.pem root@110.239.69.17`

#### Petunjuk Instalasi
> Update and Upgrade Software
`$ apt update -y && apt upgrade -y`

> Install Library
> `$ sudo apt install -y python3 python-is-python3 libbz2-dev liblzma-dev bzip2 gcc zlib1g-dev make openjdk-17-jre openjdk-17-jdk`

> Install Software Pendukung
> `$ sudo apt -y install sra-toolkit bwa samtools`
> 



### 2. Instance GPU Based
#### Minimum Hardware Requirenment
- Access to the internet.
- Any NVIDIA GPU that supports CUDA architecture 60, 70, 75 or 80 and has at least 12GB of GPU RAM. Parabricks has been tested on NVIDIA V100, NVIDIA A100 and NVIDIA T4 GPUs.

####  System Requirements:
- A 2 GPU server should have at least 100GB CPU RAM and at least 24 CPU threads.
- A 4 GPU server should have at least 196GB CPU RAM and at least 32 CPU threads.
- A 8 GPU server should have at least 392GB CPU RAM and at least 48 CPU threads.

> Please note that Clara Parabricks is not supported on virtual (vGPU) or MIG (Multi-Instance) GPUs.

#### Minimum Software Requirenment
- The following are software requirements for running Clara Parabricks.
- An NVIDIA driver that supports cuda-10.1 or higher. If you're using an Ampere GPU, support for cuda-11.0 or higher is required.
- Any Linux Operating System that supports one of the following:
- nvidia-docker2
- singularity version 3.0 (or higher)
- Bare metal installation is supported for Ubuntu 18.04 only
- Python 3

## Spesifikasi Komputasi


## Kebutuhan dan Analisis Biaya

## Referensi untuk materi pelatihan:
1. https://github.com/sib-swiss/training-collection
