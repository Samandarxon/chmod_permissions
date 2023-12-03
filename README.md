# “chmod” in Linux [mode]
The “mode” helps in setting new permissions that have to be applied to files or directories.

This mode can be specified in several ways, we will discuss two modes: Symbolic and Octal mode.

Linuxda 2 xil mode bor 

1) Sembolik mode
2) 8 lik sanoq sistemali mode

             1.  SEMBOLIK MODE

	Operators	Definition
	`+`		Add permissions
	`-`		Remove permissions
	`=`		Set the permissions to the specified values
	
	(UZ)
	Operators       Definition
        `+`             Ruxsatlar qo'shish
        `-`             Ruxsatlarni olib tashlash
        `=`            	Belgilangan qiymatlarga ro'xsatlarni o'rnatish



		Letters		Definition
		`r`		Read permission
		`w`		Write permission
		`x`		Execute permission



			(UZ)
                Letters         Definition
                `r`             O'qishga ruxsat
                `w`             Yozishga ruxsat
                `x`             Ruxsat berish





		Reference	Class
		u		Owner
		g		Group
		o		Others
		a		All (owner,groups,others)





			(UZ)
                Reference       Class
                u               Egasi(USER)
                g               Guruhlar
                o               Boshqalar
                a               Hammasi (Egasi,guruhlar,boshqalar)





		Examples of Using the Symbolic mode:
	Read, write and execute permissions to the file owner:
            chmod u+rwx [file_name]
		Egasiga o'qishga yozishga ruxsat berish 
	Remove write permission for the group and others:
	    chmod go-w [file_name]
		Guruh va boshqalardan yozish ruxsatini olib tashlash.

	Read and write for Owner, and Read-only for the group and other:
	    chmod u+rw,go+r [file_name]
		Egasiga o'qishga yozishga ruxsat berish
		Guruh va boshqalarga yozishga ruxsat berish.




		2. Octal mode
	It is also a method for specifying permissions. In this method we specify permission using three-digit number. Where..

	First digit specify the permission for Owner.
 	Second digit specify the permission for Group. 
	Third digit specify the permission for Others. The digits 
	NOTE: The digits are calculated by adding the values of the individual permissions.


		Value	Permission
		4	Read Permission
		2	Write Permission
		1	Execute Permission




Examples of Using the Octal mode:
Suppose if we to give read and write permission to the file Owner. Read, write and executable permission to the Group. Read-only permission to the Other. They our command would be.

##chmod 674 [file_name]

Here.

6 represent permission of file Owner which are (rw). (4+2)
7 represent permission of Group which are (rwx).(4+2+1)
4 represent permission of Other which is (r). (4)







