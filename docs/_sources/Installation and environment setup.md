# Installation and environment setup

As part of this protocol, all analysis steps are carried out using Python, an interpreted, high-level general-purpose programming language that can be used on a wide variety of operating systems, including LINUX, Windows, and macOS. Currently, the protocol is written in Python (`v3.10.4`) on a Linus-based Linux system (Red Hat Enterprise Linux version 7.9 (Maipo)). The protocol can be run on most UNIX and Linux distributions, however, Ubuntu 22 and Fedora 36, Red Hat 7, and macOS Monterey are recommended. Besides HPC devices, this protocol has been tested on other devices, with the following specifications:

::::{grid}

:::{grid-item-card} OS!
Windows 11 (5.10.102.1-microsoft-standard-WSL2), and Fedora 36.
:::

::::


::::{grid}
:gutter: 4

:::{grid-item-card} RAM!
16 GB 
:::

:::{grid-item-card} SDD!
256 GB 
:::

:::{grid-item-card} CPU!
Intel i7
:::

:::{grid-item-card} Conda!
v4.12.0
:::
::::

## Clone "Pathak" GitHub repository

````{card} Open a command prompt or terminal window on your local machine.

Here are the step-by-step instructions to clone the "Pathak" GitHub repository.
^^^
1. Navigate to the directory where you want to clone the repository.

2. Type the following command to clone the repository:

```
git clone https://github.com/nilesh-iiita/PATHAK
```

3. Press enter and wait for the repository to be cloned to your local machine. This may take a few moments depending on the size of the repository.

4. Once the repository has been cloned, you should see a message that says "Cloning into 'PATHAK'..." followed by a list of the files and folders in the repository.


+++
You can now navigate to the cloned repository on your local machine and start working with the files.
````

## Here are the step-by-step instructions to download and install Java 1.8.0_202

1. Go to the Oracle website (https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html) and click on the "Java SE 8 Archive Downloads" link.

2. Scroll down to the "Java SE Development Kit 8u202" section and click the download link that corresponds to your operating system.

3. Read and accept the license agreement, and then click the download link for your operating system.

4. Once the download is complete, double-click the downloaded file to begin the installation process.

5. Follow the prompts to install Java 1.8.0_202. You may be asked to specify an installation directory and to choose the components you want to install.

6. Once the installation is complete, you should be able to use Java 1.8.0_202 on your computer.

7. To verify that Java has been installed correctly, open a command prompt or terminal window and type the following command:

```
java -version
```

`````{admonition} load Java on HPC
:class: tip
module load Java/1.8.0_202
`````


## Create conda environment

````{tab-set}
```{tab-item} Fedora (37<) and Ubuntu (22<) and WSL2
[environment.yml](https://raw.githubusercontent.com/nilesh-iiita/PATHAK/main/environment.yml)

    conda env create -n sparknlp --file environment.yml
```

```{tab-item} Mac OS
[environment.yml](https://raw.githubusercontent.com/nilesh-iiita/PATHAK/main/environment.yml)

    conda env create -n sparknlp --file environment.yml
```

```{tab-item} Windows 11/10
[environment.yml](https://raw.githubusercontent.com/nilesh-iiita/PATHAK/main/environment.yml)

    conda env create -n sparknlp --file environment.yml
```
````




