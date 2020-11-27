
In this file we will mention existing pdf libraries and which one we chose
The choice will probably be based on lightweight, speed, cross platform operations 
and ease of use


 | Library Name  			| PoDoFo | MuPdf | QtPDF       			                            | pypdf | 
 | ------------- 			| -------|-----  |----   				                            | ----  |
 | Open source   			| Yes    | Yes   | Yes   				                            | Yes   |
 | reads from images     	| Content| Yes   |yes    				                            | Yes   |
 | pdf concatenation    	|  ?     |  ?    |  ?    				                            | Yes   |
 | specific page deletion   |  ?     |  ?    |  ?    				                            | Yes   |
 | specific page rotation   |  ?     |  ?    |  ?    				                            | Yes   |
 | Problems				    |  ?     |  ?    |  requires chromium                               | Yes   |
 | comments                 |  ?     |  ?    | chromnium is actually c++ base maybe it is a     |       |
 |                          |        |       | good thing and pdfium is the part that is used   |       |
 |                          |        |       | for that                                         |       |
 |Tried on multiple platforms|?      | yes   | Yes                                              | Yes   |

It seems we will start a quick prototypw with pypdf 2 or 4 for now as it ticks all the requirements I am looking for.

However it is pure python project.  Therefore, this can't be the final version.

Other than the libraries mentioned above This blog post lists a number of opensource pdf viewer projects on which we can base our manipulator https://www.goodfirms.co/blog/best-free-open-source-PDF-software