
In this file we will mention existing pdf libraries and which one we chose
The choice will probably be based on lightweight, speed, cross platform operations 
and ease of use


 | Library Name  			| PoDoFo | MuPdf | QtPDF       		  | pypdf | VersyPDF| Cairo  | libharu |
 | ------------- 			| -------|-----  |----   			  | ----  |----     |----    |----     |
 | License                  |        |       |                    |       |         |LGPL/MPL|         |      
 | available in vcpkg       | Yes    | yes   | No                 | No    | No      |yes     | yes     |
 | Open source   			| Yes    | Yes   | Yes   			  | Yes   | Yes     | yes    | yes     |
 | reads from images     	| Content| Yes   |yes    			  | Yes   | Yes     | yes    |         | 
 | pdf concatenation    	|  yes   |  yes  |  yes    			  | Yes   | Yes     | no     |         |
 | specific page deletion   |  yes   |  yes  |  yes    			  | Yes   | Yes     | no     |         |               
 | specific page rotation   |  ?     |  ?    |  ?    		      | Yes   | Yes     | no    
 | Problems				    |  ?     |  ?    |  requires chromium | Yes   | Yes     | it does not natively read pdfs
 | comments                 |  ?     |  ?    | chromnium is actually c++ base maybe it is a good thing and pdfium is the part that is used for that |      |       | Yes |
 |Tried on multiple platforms|yes      | yes   | Yes                                              | Yes   | Yes |


It seems we will start a quick prototypw with pypdf 2 or 4 for now as it ticks all the requirements I am looking for.

However it is pure python project.  Therefore, this can't be the final version.

Other than the libraries mentioned above This blog post lists a number of opensource pdf viewer projects on which we can base our manipulator https://www.goodfirms.co/blog/best-free-open-source-PDF-software

For OCR I will probably be using tesseract as it includes Arabic, English, and French, which are the languages of interest.

As time goes on more things will be found out. right now basically all the above libraries seem very promoising I will choose either Qtpdf 
or a vcpkg supported library for ease of installation Qtpdf has been tried on all platforms. However it feels that dragging the whole of chromium just to use pdfium a bit extreme 

The rest of the libraries don't suffer form this shortcome The aim is to create as light as possible software that does as much as possible
Therefore the lightest of the aforementioned libraries will be chosen
