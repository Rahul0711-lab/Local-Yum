# Local-Yum
Installation Redhat 9.3 Local YUM Server
YUM is the primary package management tool for installing, updating, removing, and managing software packages in Red Hat Enterprise Linux. This is Open-Source Command line package management utility. YUM performs dependency resolution when installing, updating, and removing software packages.
Before run yum command we have to configure yum file in .repo extension.

File Path 		:	#cd /etc/yum.repos.d/
Configure File	:	#vim yumrepos.repo
			In vim file:
				[Anyname]
				name=anyname
				baseurl=file://<packagepathaddress(Appstream)>
				enabled=1
				gpgcheck=0	

				[Anyname]
				name=anyname
				baseurl=file://<packagepathaddress(BaseOS)>
				enabled=1
				gpgcheck=0	
			==============================

Commands:
#yum clean all :	To clean unnecessary files.
#yum update all	:	To update and check yum file.
#yum install <packagename>		:	To install Package.
#yum remove <packagename>		:	To remove installed package.
#yum search	:	Searches package metadata for keywords
#yum info :	Lists description
#yum repolist	:	Lists repositories
#yum history :	Displays what has happened in past transactions
