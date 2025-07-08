---
title: TripleBaka
CTF: SSMCTF
Year: 2025
category: [crypto]
author: Hal0g3n
date: 29 Jun 2025

hide:
- footer
- toc
---

# triplebaka
by [Hal0g3n](https://github.com/Hal0g3n)
> more like baka ↑↑↑↑ baka ↑↑↑↑ baka...

## WHY REV
Why are the functions so... obfuscated? Well that is how SSM do be sometimes... time to dig in

<img alt="" src="data:image/jpg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/4QBmRXhpZgAATU0AKgAAAAgABAEaAAUAAAABAAAAPgEbAAUAAAABAAAARgEoAAMAAAABAAIAAAExAAIAAAAQAAAATgAAAAAAAABgAAAAAQAAAGAAAAABUGFpbnQuTkVUIDUuMS44AP/bAEMAAgEBAQEBAgEBAQICAgICBAMCAgICBQQEAwQGBQYGBgUGBgYHCQgGBwkHBgYICwgJCgoKCgoGCAsMCwoMCQoKCv/bAEMBAgICAgICBQMDBQoHBgcKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCgoKCv/AABEIALUAwAMBEQACEQEDEQH/xAAfAAABBQEBAQEBAQAAAAAAAAAAAQIDBAUGBwgJCgv/xAC1EAACAQMDAgQDBQUEBAAAAX0BAgMABBEFEiExQQYTUWEHInEUMoGRoQgjQrHBFVLR8CQzYnKCCQoWFxgZGiUmJygpKjQ1Njc4OTpDREVGR0hJSlNUVVZXWFlaY2RlZmdoaWpzdHV2d3h5eoOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4eLj5OXm5+jp6vHy8/T19vf4+fr/xAAfAQADAQEBAQEBAQEBAAAAAAAAAQIDBAUGBwgJCgv/xAC1EQACAQIEBAMEBwUEBAABAncAAQIDEQQFITEGEkFRB2FxEyIygQgUQpGhscEJIzNS8BVictEKFiQ04SXxFxgZGiYnKCkqNTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqCg4SFhoeIiYqSk5SVlpeYmZqio6Slpqeoqaqys7S1tre4ubrCw8TFxsfIycrS09TV1tfY2dri4+Tl5ufo6ery8/T19vf4+fr/2gAMAwEAAhEDEQA/AP3UrnMwoAK3lIAGcRf89P8AlhXLOQHzH8Sv2kPGXxvvL74cfs0eIH0vTrWeW18QfE2CDzfJl/5a2elf8sp7vOfNm/ewwzfuf3037qLjjuBwem/2hoc3/DP/AOzX4PtYtbtP9K1PWNY+1y6fonm/vvtmoSzfvrzUJf8AXeTLL503+um8mHyZq3hugPoz9lr4FeEvhN4PkvNP1afWNf1WYSeIfFOokS3Wqy5zF5v/ADxii82QRWkX7mEdMcmu9bGh6xTAK0mBzPxV/wCQFbf9fv8A7RrnmB8zfGD/AJLn8N/+wXrn/om0rl9oL2SLH7KH/JPNW/7KD4m/9O93R7UPZI+ovBH/ACLVl/15RVtHENi5UjVrpjUk0PmjcZN54h8iC382ojiMRN7FyjhoLc8O/az/AGof2cPgf9it/jF+0h4D8Jf62KCDxJ4ttLCaWX/plFNXRDDYur0OaWPwtNWufDX7SH/BRH9jeH4q63q9h8aP7ZttR+Ekul2V54b8MarqkX2uWab9z5tnaTQ12R4dxb1seN/bGGvudl8Mv+CxH7DGheCtA07VfHPjf7Tp2mWkU/8AxavW/wDnj/16V1Q4dxbtoJ55hY9T2KD/AILtf8E2iI/7V+KPiy1jih/5a/CTxNJ/6J06tMbwxiYwu439CcPxNRqysmfSXwO+MXw5+Pnws0n4t/CXxRHrXhvWYPM0nVGhMXnKJTDJujMUZim83zYjGf8Anl614Lw0sHJpnv0MTHExujsJvtEx+zwfuv8Apt/zyrE6Jnyt8ePgf4i+HXj+++JP7OsdhHLd3EV/4m+Hs08MVrqssvEt3ayzARWd3/5Buz/rfJlm+2UHPM8+8N6prB1iT9oj9l7UItL8Sef5Xifwr4kgltbXWvK/5dL+L/XWd3F/yxm/e+T/ANNofJrkrTJ5j6e+A/7Qfgr4+6HdX3hr7VYarpF79m8TeHNYiMWoaTdk8wyxf+1Yf3M3+thlloozQ+Y9DrcYUAVPEGt6b4d0648QatqMVpZ2kPm3d3M3+qi/66/8sqUpWQXPk/x/8ZfF/wC1pfTaH4AuNU8OfCozSxT6xZ+bbah4wGSZfsph5s9P5/1v+tu/+uP+u5ZTT2C5j6B8cPhP4c+JGk/s/wDgfR/+PTzrD/iT2XlaVok0Vn539nf88fN8nzf3MX+p/wC21ZwTYNpG/wDs6wf8V58Wh9o/5qDaf9sv+JFpFdUITutCeeHc+ovhjAP+EPiz/wA95a7uSS6F88O6N/yBT5Zdh88O4lXOMuw+aPc5j4p/8gCL/rvXPNMLqx8u/tFa5o/g74teBfEHiPxBYaXYxaX4h8/UtSvYooov3Np/rfOo+qyfQ5ni4rqcB+zh+2z+yfpXgnV9P/4XRo1/c/8ACaeJpfO0Hzb+LypdXu5opv8AQ/8AntD++prCTfRk/XI9z1/Uv+CuH7Fvw08L7r3xB451OezsQfsXh34S+JLp5/Yf8S/y8/WTFdlLLajekTnqY2Pf8T4K/aq/4OY/jnHLdaJ+z9+z1a/DuDPlRa98are6F/LF7aePKihl/wC203/XKvcoZRzJcx5lbMbNpM+KfjX+3v8AtsftIiVfjD+1d8QNesZrfzDpum+IP7L0/wAmX/ljLa6b9kim/wC2vm19Zh8jwkWnY+VxGb4qV0meU+Fri58H2f2DwfBa2McX+vis7KKKKvdoZZhILY8GtjcZOW7Oks/jF4wg/wCP64il/wCu1etD6ttynm1XiUviN/R/jFo8832fXNP+yy/8sJoa6ofVv5TzKtbFL7R1sN9bzwxahBbxSx/89v8AnrXZWwFGrSehjg8fWhW1Z+q3/Bvh8VDqvwK8ffAC+uLbzfBHjn7fplnF/wAsdP1WH7X/AOnD+1a/D+LMIsPiXZaf1/XyP27hnFuvSWtz9BK+QPsJHmHxP/5GSX6Unsc8z5cvPiPp/wAK5vit441Xwvf6zHD8W7S1g03TYPNuruW7s9DtIvKi/wCW0vnS/wCp/wBd/wA8a82vJ3OW5peRo/xUs7L9oD4A/FCKw8SafB9l0XxJZw+bFL5X+ts9Qtf9dNF53m/uf9dD/wBdvOpUZMLn2pXdzHUc/wDE7x/4H+Ffgm++IHj/AMQWul6bp8Pm3t5ef6qjmA+W/HWveMP2n76TxJ8XdPutB+H1pL5mm+BNQ8oXOomLE32zVRn/AFXA/wCJd/qh/rZf3vlQxZyvVpNHLVi5VtDzH9on40eP9W/Zw8Y/GD4SQXVp4A8J+H7u/wD7e8/7LdeJZYof3WnaV+5/cxS/6n+0f+/Pnf66ryfKp169u5OZVPYUL9j4Z8SftpftMa5pugaf4H8QeHPAekeE72WXw9D8N/DH+q82GaGWbzdSmvPO83zZf33/AE2r9hwPAkIJNn5djuOZSvFHAa98TvjBrl5qWseI/wBoj4jRXOrXv2rVJrPx1qFrFd/uYYf3trDNDF/qYoq9xcLYektkeJ/rRXqu9zynxh4x8H67P9o1XT/7euf+fzWIPtX/AJFm86uqOTYWC2QpZ1ipvdnHaxqvg+CzkuJ/C/hywtv9VNNDpcX/AMZrzsXk+GfY9PCZxiY73PZP2fP2Zf2wfFNpbah8MvGHiL4X6JL+9/4ST/hJ9Q0a6l/6bRWtnNDLN/218qvn55TQqaH0H9s16Z9r/Dfw5+0P4H8KSeDviL+3N8Y/GVjL5Xnxax47miii/wCuUsP/ABMIf+uP2qWuWXDNOTuhPiWqlYkh+Ffw/gvLbxBqvgewv9StP9TrGsf6fdRf9NvtV5++hrupYGMdLHNUxrkr3Ol/0if/AEie483/ALb+bXpU8NTS1SPNqYmbe42nyQXQOeb6jJ4Le+hlt763822m/wBdT5V2FzS7njPxY/YM/Zf+IsNzqFl4Gl8J6lN/zEvBQ+wed/2yh/0Sb/v1LT9k46midj5Q/aE/ZI+J37PllJ4g1qH/AISjwnznxHpEEsMunjH/AC9Wv77ye/72KWWH/nr5VHt3B6j5YyWm/wDwO/36em5xng/x/rHhyGI29xLdWMv+uh/5ZS/9cq93A5nC9meJjqUpo9Q0b/hH/Edn/aH2eKX/AK7Q+b5VfRwrU60bo+blSnGWpZh0q3t/+QHbxRS+fD/qYfKrWZzz0R9w/wDBv542Ph39tbxt8OMHzPFnwr/tSc++lajFF/7ma/HOP7Jn7F4dqUo3Z+vf/LH7RzX549j9Ie55d8T/APkY7n/rjWExHyN48H/I9W/2f/W/tH+E/wD0s8L1lZGfIemfFT4EaxBr198YP2eriLS/FOo/8jDpupT+VpXiv/r68n/U3f8Ayx+1xfvv+e37miyDkPd/jh8b/BfwL8OQa94wup/M1GY2uj6ZpsMtzdandcGGCGKHmYnP+qHockRCWWubmGfMPifVLy7u5/2iP2qdYtrCHRpftPh7w2zGaw8Kzf6mIkxHN7qJ/wBUTFESf9VaRf8ALaZNsRY8N/Cvxh8d57bxB8adHl0vwd5/m6Z4Dmh8q61v/ptqv/TL/qHf9/v+eMOlDSDQoQ5qlyt/wV00K4+HX/BNXxtq+7yZNQ1Pwzo0MJ/5ZQ3Wu6dDL/5Cllr6jh2pbFRS7nkcSy5cM7bWf5H5EzfaILP/AEHyvtP/ACwhm/1Vf0Rh5TdNeh/OOIhD2j9Tl9S8Aax4qvP7Q8R+IP8AtjZ/6qKubE+0OjDezXQ5fXbawbUo/B/w/wDD8uva3dXsVjZ/89bqWX/ljF/n/pt/qvOr57F1asVufV4OjSn0PsL9l39hnwv8I7uy8f8Axat7DXvGv+th482w0X/pjaxf8tv+vv8A13/PGvNjOtN6s9KUaMFZI+gv+W37797L/wAtpv8AnrWMcPUi73I+tU5aWG10RU4qwNU5hU8yQuVsKXtrD9iFAFO8vtQ0qH+0Nct5Yrb/AJ/P+WUVGwEesWPin/X+HNY8qX/njeQebFLR7bn0NCifGOoaH9m0/wAfaP8A2XLd/uoZpr3zbS7/AOmMUv8A8dodHmA+R/2zP2LrfwP9p+OHwI0/ytE/1vifwrZwfuoof+fy1i/55f8APa0rGMHSloypUYzjqeC+CfHH/COalHqEHm3Vld/6/wD6aw/89q+ky/EuyR81j6Cg9j2PTfs995c8H72L/WwTV9NJ3R87U03Ppr/gjX4I+L2uft7f278JviZp/hk2ngU3XiS58QeDP7Yi1PSv7QtPN0+2/exSadLLLLH+9jlxMYR+5m8n91+Pcf25kfsXh22oNH7ec+d9o/65fuf+eVfnb2P0h7nl/wAT/wDkY7n/AK41hMR8jeNv9b42/wCzlvCf/pX4drM05T6v8H6Hb+I9Y/se+uJf9T/yxoDlPnDWL7/hB9ej+LHxp1CXxb8UfEP+gaLo+g2X+q/566dp9rN/qYv9V513N/0y87yf3MMPJGjqcZ1nwy/Z68YeIvG1t8UPjTcfb/FNp/yL2j2f73SvCnm/88pf+W135Mvk/a5f+2P7mumFET2Pp7wf4B0jw5Z/aNUn825i/wBdNV0aLWOdjRTvgD5X/wCC7Ug/4d9Xkfefxz4ZP5alDL/7Tr6jhyKWeJHgcTRvkbZ+OFmf9Vb/APPav6MoVY+zSP50mm6jOS+KnjHULCH/AIRex8qKW7/57V89mtZa2PZwNBto92/4Jz/A7SPBngqP9qbxyPJuvEFl/wASCa9m/wCQfpX/AD1/663f+t83/nj5VfHKpd3ufbSjyLltax9J2U+oatZx6xb6PLa2N3+9svtkHlSyxf8APbyv+WMNdEZHPMvf6Pj9xVXYrIIen4Uhj6AMrxJPrFjZ/wBsaF+9ktP+XP8A56w0A9izo/iPR/Emj/8ACQaHb+b5v/f2Kb/njWkjJbhoPiPR9Vh/tCx8q6tv30V7DeQeb/11hlrnnszoiZviTSrn4Ow22s2OoXV/4J1yfytMmvJ/Nl0S7/585f8Ant/0xm/5bQ1jh5cr1Op2sdRpuq6f5Mun654ftdU0nUYYYr3QZv8AVXcX/tGX/pt/yxroqzcloc73OS8X+F5v2bPEGnJb6zLqnw88SiWXwzq80P760/562kv/AE1i/wDasU1eRLEe+1fVHbToO1z4W/bB/Zz0/wDZz+I9t/witx9l8FeJvOl8P+dN+60+7/5a2n/XL/ltF/21h/5Y16mDxfKc+JoRZifBnxHb/vPD8/8Arf30sP8An/yNX2eFxkVS1Z8fmOWznUVj9Uf+Dd/4cm9u/jN8b55hLYwz6V4T0yLvFLawy6jdTf8AbWLVLD/vzX5JxpiVVxFk/X9D9a4Hwrw9BXR+n8P2jzorie482vi3T0PtXueX/FT/AJGm6/641zzp2EfI3jb/AFvjb/s5bwn/AOlfh2uWMtRVpH158MufGNv9K6YyVgoyPjX4Vn4gfDm8ufFF98cPhBr3ijXJvK1PxJqU8v2uWL/llDFF9r/cxRf88Yv/AEd51cUaruYHqWg/tX/GDw5Z+RY/Ej4I+Z/y3m/0vzZZv/AuuqFZil8LNH/hsz44f9FR+CX/AJN//JlXGr/txlTk/qJ8o/8ABY/9rb4q+Kv2NdS8D6xrPg7WRd61p1/DN4I8Mahfxaf9ku4bvzr+X7X/AKHafuv9b5Uv/XKvXyLFOGdnHn9OMsk1/D+v68j4Lh/1MdxP5UVzFP5s8MP/ACyr+g6FaTp3R/OXL+9afc8z8P8Ag8/H3456R8MVOLfxD4h+y6nMD/zD4ofOu/8AyDFLXzua1nezPrcso7NH6R/D7RNO+JvjHVvF/iPT4v8AhXngOCLzrL/llreof8utp/1x/df9+Ya+cVS7stz25JpHQaxfXGq6xc6xff6yWf8Af11xmc0yuPtHkS/Z/wDWV1AZuj31vfWf9sQf6q7/ANR/1x/5Zf8Ax7/ttQBcoAvQ2N/PZyahY+V/on+v86i6CzaPONOnuPA/xal8H/vfs2uf6jzv+etXNoyXUk+IRuPA/iSP4kaH+9sppvK1qGsJnRFo9K8HXXhfxlpt58PPF02fCvimyitbu8/58B/yy1Dt+9tZf/IXmxf8ta8zEXjaUVqtv8vn917Podieluh5z4GbxN8NfF2q/Ar4hwCPVdFvJba3ilP+uli/5Zf/ABmuvDVI1I3vuc0k1LY9d8I6TYfGHw5rX7OXiK4tfs3iv/SvD80x/wCQfrcX/HrN/wBcpf8AVS/9doq8/F0uT31039P61/DqdtKtpY+V/Gnwsn/aS+BPiP8AZ48SzS2Ovww+b4fF5/rbXUIv9V/36l/1v/TGaWroxl0MKtdKauro+C/DWq+L9Du7LxBY6vFdRw3v77Tbyz8qXzf+eP2qGH/rr/yyr044upCm0aKlTqtM/Vn/AIJE/wDBSLwh4J/Z/wBL/Z10j4ifDrw/4ua8u9T1PSvHUF1YTXV3d3c02Yboy+TeeTF5UX7qX/Uwxf6qvzjiGrKpWbPtcnksPGyPtSH9tD41TkQQeNPgvL5PaG9uv3f/AJN14brtI+jTuc5rH7Sfxw8Vax/aP/Cc/BuL/tvd/wDx6ueVdgcteeB/EGq/DfxB4on+IHhL+0tR+IOneLYLyz/5BVpNaTadN9j/ANd/1D//ACNXJGTuc1aTZ1OhftJ/Fjwrrv8AaA+KPwWk/cfvzN9r/wDkuumMgoyZ9B/Df4K/Befw1+/+D/hf/XS/67w/af8AxmuqyOk6j/hR/wAEP+iP+E//AAmLT/4zTsgF/wCFIfA//okHhH/wn7T/AOM1pZXM+Q4z44fs6fAHxV8Pr7whq/wW8I3Nlq0M1heQy+GbT97DLDNDLD/3682qg+SakiZ0+aDiz8J/2l/gR44/ZC+J3ij4L+Krm6uo9Eg+3+H9evPK/wCJ1pP/ACyvPN/56/uvKm/6bQy/8sfJr9nyPiFVcPyvsfifEHDbhieZdzzz9g/VLe9+LXin4kaJrHmx+GfCU0UN5D/qvtd3NDDF5Uv/AC2/1UtcGNxSrVGevleFeFopM/Tn4geFbn4PfCbwV8ALH97JaeH4fEXiD/nrd6tdf/GovKrhyhc0ZSfp8l/wb/gdWNknHQ5jTbHz9YttPnt/K86b/wAgxfvrv/yDFLWv/L48NxbZz/xD1UaH4JvdQ/7Zf9/a9JNWNeQJoPsOpeH/AAv/ANMJZf8Av1DRdByG5/7WrWMk0ZSi0zf+Fk+kf8JrbaR4puPK0nVv9A1Ob/nlFL/y2/7ZTeVN/wBsa8zF8yu4npYZprU8g/ah8Oav4W12L9x5epaJqd3YTQj/AKZf5/8AINHtVO0k9DN0XFOJp+EPGHgj47fDe+1Dw7qHmxzTXdhe/wDLLyruKbyZf/I0VaOrDELlTOP2FTDS5mjN+BuuXEOj33g++uPKudD/ANTDXRVpJxNKdR3Om/a3txLoXgr9ofQgItRtD/wjuszAf8trX/j1m/7bWn7r/t0rxJYeUajS23+//g6/M9GNROOpf8K679u06y8UeG9Q8rzvJurKb/n0l/8A31evPBv2FzmpbmR8dre30L9sseN9DtvskXjzS4tZ8n/njLdQ/wClf+TcV1XLlK9hNxfT+kFZJux4Z8OP+CV/jf8Aa9/b68T+EfDniqHw54FtLPT/ABP4u13TM+daf2hNdxfZLCL/AJ6zTWF3L5sv7mHzf+2M3zHEXFU8si9D7LI8gpVqV7n2J4g/4N3v2D/ENn9gg8YfFCwiu/3Xkw61p91F5X/TXzrSavgI8XSzGb0PtMBw3CnJtnDal+zH+0Z/wR10mPxL8EbrSPj/APBTQrLztY+HXxM0C0HiXRNPBHnXWl6pDAciICOT7HLCIvKj8qGLzpawwmbU8XW9n1N6uAeFpOfY+vPhX4w/ZA/a2+H1j8YPgf4Q8L3+iXflRT2d54YtPN0+7/5a2d1F5P7mWL/2t/y2hmhr2sbhp4aip23PKw+Mhi6jhc8c8d6H4Xg8N+O/D9j4fsItN/4aC8M+dpsNl/on/H54d/5ZV5kabjuY9WfT3g/4O/B+fxVbf8Wf8L/67/lt4YtK6Y+8jeJ6t8K/+Rc/7b1sbHRUAFaPTc0Ub7HE/tBePfB3wx+F974/8feKLXRtD0P/AE/U9YvLzyorSGL/AFssstXCDnJJET5YQbZ+BX/BVn9sbxB+274x025tvC8WjeCtE+1xeEdOvLLyru6il+yebNdf8tf3vlf8en+p/wBT5sUs1fqeS5I6NDmfU/KM1zpVcTyxMz/gmb4WHir4j6/o8H/Htq3iHwRazwzf8soZdR1Hza4sbB0arRpCpegrH6CfHzxE3jD44+LPEBP7v+2pYoT/ANMov3MX/kKKtcoTVHU58RKTOb8FXK3viTUb+4P/ACBfCWo3Vv8A9dpZrTTov/S+nOSjXs+v+Tf6HPThzHC/GyfyPBP2f/lpNexRf9+q602yuVGJ+0V8Rrj4SXnhL4g/2PdX9lN4h+y6pDpsHmyxQ3f7nzov+e3leb/qaTmo7jUG9j0iznt76zi1CC4822u7LzYJvP8AN82H/ll/12/67VrQqKexnXpuO6K2m33n6ve6fP8A8sp/3H/XL/llTrxTTFh5e8kav7f8A12y8N/E4DzZPEtlp99e8f8AL3++tLr/AMixf+Rq8KNXkwM3/Lp+q/Bo910VPHRj3POfhx4HuPhJ8Jvg58Z57eWx0D4heC9Ei8T48r/iVeIbuHztPm/c/wCp83zf7Olm/wCe0Okw/wDLavjcm4gc8xdNvqfWZzw/CGXqaXQ5L4qeMbf4IfEOX4of2Pf3Vj5EP23TdHsvNlu/N/c/uov+W3/bL/ltX6Q8VeJ+fU8K+a1jvp/jR8P/AIqfDjxr8MPAGr/29F/wjFp4jm1Kz8r+z9Plimhmihll/wCesuny3U3kxf8APb/ptDXLOopSUl0/L+rHfHD8kNTA/Z1+JvhfVbzW/hR+9/tLwzZWl1Mf+mV15vlfvf8AtlLXfhsbGvScb6nn04SWrWgftgX3kTfDP7DcSxalaeJ9P0v/ALdP7XtJv/bqX/yLXPQtGqyKvc+q/wDgnL4wt/Cvx+8f/C/VbiLzPE/hjTtZ0vzv9bL9kmmtNQh/65Q/atPm/wC3yWvzPjOhDExeh+h8I1J1IWbPsaH/AFP2evyzBxhhajR+k0OeF2ct8YNLOq6JGp6eb++/65Uoc2CziCWzZ0UIxx+Vzb7H4e/so/H74gfsI+PIvFHwr/4mltp0MWg+J/B80/lRa3p1p50P+t/5Y3cXlfuZv+m3/PGaav6djkNPMcjhVt0P58lm8svzqVO/U+9PCvxi+H/7Qvwl1/40fCzUPtWgeIfj34TlsppoPKli/wBM8Owywyxf8sZYpopYfJ/5Y+TX5fmNB0G1Y++pTjON0z7l+H3/ACPVr/12lriwjUjrWh13wq/5Fsf9d66zY87/AG4bT9sPTvhKnj/9i/XtK/4SPw3ffatU8H65pkV1a+JdPxiW1iPnQ+Vd4Alh/exRS/6mYxed50LW4nsfP3wW/wCC0Pg7VPDFpr37QPwc17QtKuJ0tT4w8H2s2saXayg/6m7tvKi1HTbr/XRSwfZJRF5RzN+7Nd88uni37mp50cwhhE+Y+Mf+Co3/AAUUk/bo8cxfD34N60f+FP8Ahm+83TpSfL/4S/Vov+YjKf8An0h6Wn/LKaYed/yytK++4a4ZqR5ZTR8HxJxLHWEXqfFPxy/489J/1sUX779zNX6Pm+BhTSSPznLcfOpV1PTf+Cb+t3HhXx3428Q6T/rdEPhPWYP+3S81GavgM4o8tj7/AA9ZOkmfcF5qtv4j1K51Cx/49rvVJpYf+uVdlGklFGNbFqZd8H3wg07x/wAf8wXSbD/v7eTTf+2tc+IpJyQU/eizzf45WIvfhv8AaBby/ub2KX/X/wDbH97/AN/aqpWWBjdnJl8JV58jPOPF/wAY4Pin+zrbfGibwhqmg+JPD2l6f48g8N3kMUt1/os0OoxTRf8ALK8h82L/AF0X/bbyZoZoa+UzLMY4lN3PqsPgZ4Gal3PpD42fA63/AGWPF2kwWNj9q+GfjGfzfCN3D/qtF1CX99/YUv8A0xl/11pN/qf9baf8+kMvk8NZ5G7Umetn2VOdK8UcT42GoeAPiRpuoarb+VFqMH2Cf/0daV+i4OUMY20fCUsPPDVNSf8Abdl1Hxx+x54T8D6Tr/2DUdR8W3fhfS5v+m2oTWkNr/5N39fNZzXjhMtrR2TX46p/gke/l9KWJzCEkfaWj/AzwN8Ufh14g+D+uaVcjwxqPh06DLZ2l55csUUv/PKQf6qWHyvNhl/5Y/63/llX845LXnDO5zvpc/bsbCnLLIwe9j83PFfw/wDGvxy/a18EfsI/8JdJceI9A+IkVh4z8d+Fp4eItPlm1aK8tcRTRCaU6LN5uYpYbS7+1WmJpYq/Z454q1GyZ+cwy/2VfVHoHxs8H/A/9nr4neNv2eP2evHFhdaJFBLL/YOm61LdS6Jrfk/a9Q0i6lm/febLF5uowzTSzTTf6XD/AMsa68qzWMJPmZyZ7lkqsFynL/Af4dXHg7w34F+NF9BFay/FP/hIZZ/+nuHzrSbRP+/unWt1N/2+S1nw5mcaudtX6mea4B0MmvYi8ef8VV+1d4E8LwXH/IO/tHWb2H/nl9ks/J/9HX9rN/2xr7jFe/masfHP/kVs9J134s6l+zfe6b+1Lo+kXN8fh95up6zpFr/rNV0TyZodQtD/ANNfK/fRRf8AP5Daf8sa8TiXA82EbselwpiXCqlc/Rj4bfEHwP8AFfwbYfEL4deKLbWNJ1CL91d2Y/dE9Jeo/cy/8spYv+WU3mxf62vwb6u6eKlc/ZqWI9pSRn/HjxT4X8D/AA51LxT4q1D7LY6fBLf3t5/zytIv30s3/fmKopU3i5xpLe50Sn9Uy2b8j8DfCuq6hrnhux8Uarb/AGW+1CGbVNTs/J/1V3d/vpf/ACNX9j8J4P2XC8KUt7H8o8TYt1c1ly9zv/2ev2hNZ/Z78V22nTX/AJ3gHXPHfh6/8afbP3X9lfZNX06b+1/+mPlQ2vky/wDTH99/y6V8dxZkKq024n1PCeayjNKTP1u+Kn7eX7LP7OHiW00v4pfEq1k1yNYpB4W0GyOqarJFN/y2+y2UUs3lf9NpSIq/MKOSVKNRn6fWzGFamrH0f8Kv+RbH/XeoPQOmoA/Hz/guZovw4+HP7SVt4P8Agl4uudF8QfEbwvLffGLS7O3iEN1p/m+VFef9Mbu68qWGX90fOis/+WUvled91wrTVaraWx8JxROVCm2j4o1LVdP0rTftGq/6LZWkP7+bz/Kiih/9FV+wqtQwdC6a0R+PulXxmIs09Wekal/wS9/b/wDjv8HpfjD4P/Z3li03Tv3tlpuvTfYNa1uH/pwsJof/AErlim/6Y1+Y4vjP6xieTm6n6dQ4NWHpKaX4Hlf/AAT21Vb79o668P2Nxd2tn4n8C6rYXk3keUIpfOtJov3X/TLypf8APnV016/1ukpLU58Rh/qvu2dz7B/Z18R6x4j+G9to/iq4i/t/wze/2N4nhh/5+4v+W3/XGWGWKaH/AKYzRVrSrytoY1sHyK7M34weMdH8HeNrbQNb+OF14I/4Sb7JpemTwzWnlahdxedNFDL50M0P/LWX/M1cuJxSi9S8PBt2SM298R/GDxHN4g+E9jceDfFupaJ/yGtNm/tDQdQii/10U3lTed53m/8APb9zD+5l/wC2PBjMTHGU9GaYuhPLMfGy0Z6z+yFqPwV+N/7BFr8A/wBq74deN9H1Pwv4r1y0svEmmeE7y6GiSm7lmtfK1TTftcNoRaXUUMpu/wBzLzDLFNnyT+YZzjZ4KbSP02nhIYzBQmt9D6T+DvxT/Zb+KnhDRP2Ede+KGgfE/RLvwLFo2i+L4PENpqFp4rutPtP9KtP9Dl/0PUYvK+1+T5vneTF5sOfJu/J8fA1J4WPMn5nvVsNGvSSZ84fGbwfJ/wAK00jw9rfiaTXvD2rQRf8ACpfifeReUdfil/1OkX4m/wCPPVYuYYvOihhu/wDplNF9kr9G4Zz5p2kz4bNcpUZNpHC/si+KviR+0n8YPDfw38cfD+6sLb4W/EHXNZvdYhh83StQhis4YdPh83/n7866tZpof+nOKb/njXzvF+cP2Uoxe538L5ZzS55I+5pvC3xg+MRl+FGiXGq+F/BOP+Km8VaZqnlarqsUsP8AyCNLl87/AEP/AKa6jL5M0MPlQ2n76b7Xafm2SYeM60qj36H3OJxDjaD2Pzh/4LYf8FkvgD+yNqOnfslf8E4fBvh0fFXwR4en8Jnx54d0uJYvBWnS+V52kaf5X/L1+5i82L/l0mh4zN5vlfa5bh5+zbmeDjIqNVcp5r/wSK/4IT/tveK/B3jD46ftUeLda+HPh/x1ppkGg30f/E/1CTPnRalLFLL/AKJNiWWLM374w3l0OPN/e8+Kxiw0rRey7nSqCr01dH2f/wAFDtc0/wAAQ/Bzwv4c0+1i02Lx3D5377yorTT4rObSP3UX/PHztVtYf+21ebwVmFWpn3lcnjDCU6OR6bnm/hqx/tz9qj4o+MMy+V4em0/wlZedB/y2tLOGa7m/8i2sP/bnX9CUP3mPTZ+Kyv8A2c0ZP7S2uahqv7K/xat7K5/4mVp4F1uwnh/55Xf9nTQ/+Rf3X/f6lnvLLCSOnIKTjWR+ruk/DPwB4O8b654n0Pwtbafq3iCaGXxBcWh/5CM0UXk+bL/028r9z5v+u8mKHzf9TFX854+pyY1pH7TltNzpI+JP+C6nxHv7L9hvxb4Yg1D7LJqGqaTYf9dbSXUrSa7h/wC2tpFL/wBsfNrThen7XieFJ7XNOIqio5ZK3Y/KHwF49MMsfhAaNf39zfzeXo2m2f8ArbuX/W+T/wA8v9VFL++l/wCeNf1qsesBGNFbW/Q/manl0sdmM5NaH0j8Jf2DfH3xot7kfEy9F1p0UHm6ppGnapNa6Vadf31/f/uZZv8ArjF5UXH+ql/11eFXzRYy6Z7GGwCwb91a9/v+X66aNHremWHwb/Z60rRPhh+zB8OxrXirVbqKx8PxeHtChh/tC/kH+p0+1P7nzsDzZbuX/VeTLLL5UXmy14mIhRjeT0PqsJUqzSTP2F+Ff/Iuf9t6/Nj7w6KjYFuea/tM/so/s9ftbeBv+EB/aB+GFh4is4vNl0u8nHlXWlTGL/XWt1CRNZy/9NYa0oZtWwnvRdjLFZZRxUbM+Bv2Cv8AgnT8D/Bv7ROt/HC31jWfGegeHvEF3a/Cv/hKvKlltPsk32SXUf8AUwxTTfa4rqG0m/54w+d/y2mry8y41r35OZ6+ZtgeFcOvesvuPvyY+R/pE/myyed/n/rtXybnOlV57n1Dpx9na2x+Tf7bn7D2ofst/wDBSrSP2rfBvhe7/wCES+KXiaX7D/Z1x5dhomt3WkXcuoQyxfuT/pc0UV3F/rofO+1/6r/lr+n8N5+qcFFu58BnmG1bSGfFS+t/g74wi+O+lHybHUPKsPF2m2fm/wDHp++8rUYov+etp/y1/wCW3k+b/rfJhhr9Aw2LrUFeS3Pgpv667bGR+1pB4h0rTfBPxQ8Aaxa2upaJ4n06Wy1Kay+1Wnk3fkwy+bF/y2i+yS3XneV/roZq5Mzw1HH0pSvZ2Z6WCccFNXMf9sz4M/C7TP2A/E/7Yv7EXwh13QPiqf7J0az0PQjdXV14Ou9P1eH7Xp1ra/vvscX726i8m0/0SaGbzf8AVTfvfxTAZni8PiXTquyv3/r/AD6H6XUwNLNqalFdOx8q/sM/8HIX7RX7E2reI/DXxh/Zj0HxTa+Jdai1XxNNb3k+j6r/AGh9ktLT7WTiaEHyLS1PleSB5oJyPNr1sR9XzCN5O5dLCSypWZ+iHwI/4OB/+CLX7WvjHSPEvxh0Ww8G+MtPnEuiaj8U/AlpN9lu4xxNFfw+d5P/AF1llhryamVygtDpp4zmdj9AYNF+AHx2+Dd1o+i2HhLxb8O/GUUt1d/2bLa3+la1DdzebLN+5/czebNLL/z186Xza4JxlRlZM7I8tRar8Dgfgx+xR8L/ANmbw3qWk/CNtaltdS8QS6zqUOvan9quv3tnaWnlebN++/dQ2sUP73zpv+e00tcWZRlX63OjAqNDVdTxL/gs8f8AgqJZfsp2vwn/AOCYXwum1iTWzdxeLvF+j+ILS11XRbT9z5UNrFNNFL5s3my/vov30Pk/9NvNrryelCi/ef8AX9eR52a1XVloj8w/+CXHx2/4Jkf8En/Eula5+3t+xn8cNA+Nsx32/ijx34HhhtNK/wCvC1mlE0J4i/0vyZZsniWHNfSTXNB8rOamm7XR+1/7IX/BQH9jn/goL4c1fXv2W/jNbeLI9DEJ8Qw/2Xd2EtpLMJjCZYryGH/nlL/0x/dS18hmeFnzM9OldWPiz/gqHfXEPiW21DyJbqLwn8HvEOvaZpsP+tlu4tR0i7i/9IK+m8PqSm9tT5zjafLo3oc38Df+Eg0P7do/irzYtX1b/io9Ts5p/wDl71Cb7Xdw+b/12lr9upR5GfkleXNHQ8z+LXxZ/wCEd/ahuf2d9a0eKKy+IVl4etdMu4YPKi1CXUNR+yfZJZf+2X/bavL4gm1g5HuZFC9RH7X3k/kf6RmL/X/896/nvEzX1uR+w5bG1NH5Xf8ABf3xjr8HwB8OaNolrNNHefEf+1Nfhg7afaadd+b/ANsfNlil83/pjXr8E/veI1M8vjiDnk2h8y/8EwvhJ8GNV8X+KP2mPjtr91/Yng6H+wfD/hXTv3uoa1qEsPnXf7r/AJYxRQ/Zf33/AE2r+g80qzrYqMIn5Ll9KMMtbe59IfHb9ovUdV8Kyfb9PtvDHhO08r+xfAnhuCWWKWWX91F+6/1t5dyzfuYf+e3nfua5KmHjgYc0nd9yaVOVapZI+tv+Cbf7G+r/AAp8SWnxr+NmjmL4havYmKHTZb0S/wDCK6fL/wAw7zYuJrv91++li/c/6ryv9T503xWa5ynJx6H2mW4LljqfYvwr/wCRc/7b15B7R0VNbgR3puPsX7m48r/pr/zyrLMOSNLRGuGpTctWfC37BN9f+Dv2dfhv4f1y38u98MeGLTw54nh87zfK1bT/APiXahD5v/TK7tbqGvzHM7Otex9bhYyhT0Z9Vw/v+IP9V/yxp1sV7SyMKScr3PnP/grF8QPh98M/2CfGXjn4jaf5tlaXuh/Yrz/oH3cur2kNpef9sppYpq+v4fpycoyPBzXDxlBnxr48muZ/iF4X8PT/APLKea68nzv9bX77hsVh8wpKKVnY/GKreCqP1PL/AI86J/wg/wAOPFHwQFwIvBPibw/d/wBi3kM3/IlajL/yx83/AKB8vm/67/lz87/ljaf6ryMwwdajL3Xozvw1V4tcz6Htf7H/AMYrfSvif4b+IFlcf8SD40eH9Jur3yYfK/s/XPsnnWl5+5/57QxS2k3m/wDPHT4a/PuMsuo4WlzUo6n3/CmcONTkkfTv7eX/AAUY/ZH/AGG/gDbePv2t/FAvpdXjli0TwbFpf2m71u7ij/fQxRSg+VEJP9bLKPJi82KEnnypfgMpo4nFVG09j7LMIKrDy/r/AIb89z4Q+Cn/AASY8c/8Fbvi9Yftjft0/sleDvgH8MISf+EN+DvgrwjDpms6/D/z21m/hhiu/KOIh/z1wP3MVpnzZfo8RmEYK19f6/r/AIc8ynhOVn67eCfAPgb4c+FdN+HHw68MWujeH9EsorXTNN06GKK1tIf+eMXk18zicTdnq0YyS0Rd1HUNN0SD+0dU1K0tov8AntdzxRRQ/wDf6uKhio1H7zN3SqPaLPCfi3/wU8/YZ+DhuRe/H7Qtf1aKbyptC8En+3r8S/8APExWfneT/wBtfKhrpqYynQs+ZI9LDZJXxUb+zb/rr/TPSNE8e/C79oL4GaV8TNE0hPFngnxZotrqem6dLphk/tC0mh/deZbTf9dv9VLF/wBda0hms03F9DyVgUqji9DzP4K/s3fBf9nDx14g8b/szfsZaF4EvfE0EUOtTaYYtLtdQ8r97F5trD+6H+tl/wCWX/LWufFY+dSNmehTwlN9T51/a1vv+MtPB2nz/Zftv/Cvtc+2wwzf9RHSPsn/AKS39fd+GdNyd2j868Q5qLsmeS+NtVuPB3xn0jxB/wAu13B9lm/7/V+014qL0Pyak5SWpm+PPCuoar+2N8HNPg0f7VFq3i3w9LP/ANMv7P8AF2hzRTf9+bq6r5riGVsHI+tyGN6qP1k8ST2+k+G76f8Ae+b5E3+pr+e8TP8A2uR+w5fH9yfB/wC1T+0JcfB79pzSLbwr4PsdZ1+0+GOoRQ/2jD5sVrDqt3aQ+dLF/wAtpf8AiSyw/wDbaWvuvDXAe3zPmZ8zxfib5O0z5S+HHw68A/s0+AL2CwnisdKsJ7q/vdSu5v3Vqf8AW/63/VeVFF+6/wCuMMVft/sV/ab5tEv8j8rpV5zwVkrtv+vvPXfgF8D7jxjZ237SHxo8EazpereHvip4YsPCPhXWIPssuledq+kTf2jLF/0EJYbr/tjDN++/fTTQxfn2e59KbcEfV5fl0dJM/Uj4fef/AMJrZfaPK8zH/LGvmKGGeMvOR9JHloxsjzfwL+17458K6B/Y95+yh4xk/fy/6nxB4f8A/kyn7c5fbmtL+3B4rHX9kHxt/wCD/wAP/wDyZR7dB7dCzfts+MJ4f+TP/G/l/wDLb/iodE/+WNKOMU4tMzWMcWfPHxe8b/FDQfjhffGf4c/soeKIvDfiz978TfDf9qaJLL9rih8mLV9K8m786aXyYvJu7T/lt5MXk/voZobv5vNMKsRfQ9zBZjbqes/AL9qf4XfECH+z/CvjGw1T7J+6ns4b3/S9Pl/543UX+ts5f+mM377/AJ7V839SnRldn0McbCutDqfjl8CvD37RcOm+HviZ5WqeCYvtcuteDryy8211uaaHyYvtX/TKHzZf3P8Az2+yTedD5P7338BmP1ex5mOwzqpn5H/tpeB/i/8AAf472/wn13V9ei/4VbB/wmX/AAknk/8AIf8AD1pN/on73/ntLD+5u/K8r99ZzfufK8nzf1fIsxjjmkmfmOZZe6SbaPWtevrf/hdukn91+90ub99N/qv+W3/f6vvfZqnTufJzrOjOxiaR4PNx8IPEGn/CzR7W2utE1SGXwLZzT+Va2t3pXkzafD/0xi86KKvJzLCxxeWSjbU9fKsweFxqkz608N6H+yP+1hL8M/2n/FXwfl8ZXPhSyu7/AMC/2lpn2r+yru78nzfNtf8AVfa4pbDyf3v+pmhlr+cquJrZFmM7rQ/dsNSp5/hI8rPpPR/iPqGralHbj4X+I4orv/XzXkMUXlf9Nv8AXVywxzx1bU1rYCjh4WufmB/wW60z4s6J+314KuD431608N638OYYtM03Tdau4rW7u7XUbv7V+6h/6ZXVhXmcSXwuF5orVX/4H5M/UvDrLsHjKtp2Pmy7+Gnw61rUf7e1v4c6FfXsX7o6jd6ZFLKf+/1fkEuKMYrwhJpPomz+jcNwTktZKfsV9xrQ/uLP+z7DT/Kih/1MP/LKuSFXFYutF3e6OjE0sjyOjKPsls+h+qP/AASBsvEFj/wT+8HnW+IrvWvEF1pg/wCe2ny65qEtpNz/AMsvJlimi/6ZeVX7rQoSlGKt0X5fn3/yP4q4jlCrxBOUNFdnt3xp+KHgj4KfCjX/AIn/ABK8Qw6N4f0PTZZtT1K8GYYR/wC1pfN/5Y/8tf8ArrXqUsBOpNaHz9fExji+RP8Aq3+X3bbH5YfEHx9c+OdN1f8Aaw8bzxaDqWra1afYodSvf3un6dFN9k0/TvN/56+bdSzTf9NryWH/AFMNfuHDGXrD0L2sfjvEeNliMS1uecftN+LPE03xK8J+PfC17c3enHwnqE2p+HtOzLHJaQ3dp50sMWcebF53/fkS/wDLXyq+hc7VTz6dJPD7Hs/7OvirTvH/AO2N+zfb/wBoeb/a2qat++8/zf8Aj0s/tf8A7a+dXyfF9dOiz6DhPDSTuz9MvipfXEHhu2t/tHledP5UNfgmJlzYhn7HlbUVqfmb+0vrmn67+1T4/wDEEFv+90mfT9BnvP8An7hi06G7/wDR2qyw/wDbGv3Xw+hHAUeZn5TxpOWJrcsS/wDskfCfxF8UPF+l/tC+N/2ftY8W/DvS5Yb34f6bHd6TbRa1d5Bi1G6ivbuHzbSLHm2mP3U0ubv/AJZWld3EnEEXVaizjyfL3Clqj6J8SeDvixqvgnxb4o/4VvdWupaj8W9E8UQ6DeapafavsmnzaR5v73zvKh/5B8v/AC1r4D2/NK7PpkrI9R8N/tJ/EDQ9YstQ/wCGR/GUvk/88fE+if8AyXXTCvZaDOg8EfsZ6h4q0CLWL79qj4l/9+PD3/yoo9gY+wNj/hhH/q6j4l/+W/8A/Kij2AewD/hhH/q6j4l/+W//APKil9T5HoZ1MHYx/G37Glx4V0f+0LH9qj4l+Z/qv9R4f/8AlRQsPGW50UMO0j59/aE/Zs8UaV8Tvh34o8K/tEeKLrxRNqeoRaZeeJLLSfKi8rTppvJl+x6dDN9kl8r99D/zx/ffuZoYZq87MMHDl0PSwMpKWp7X+zh8fdG8f6dc6Brlv/Zet6Te/YPE/huafzZdJ1DyfO8n/rj5UsU0U3+pmhmimh/11fJVcNKMz6SLhJFD9vD9kaw/an+HdvqPha20uL4heEoJrvwXeajN5cU3m/63TpZf+fS78qLzf+eM0MU377ya+lyjMZZbUWp83m+BU4PQ/IfV/ir428Hw+H9I0S3v9G1L4ZTfZfiDDr0MMWoafp+n6v8A2d9kli/5Y3ctp/pf/PH9zL/rq/Ycpzb+0KW5+Y4zK/3rbR6B+yD8RfFH9meNfEXje/P2X+y9O8UeH9OIl/0W11D7XDawy/8AXX7B53/TGabyf+WNepTq7031OTE4Pko+0j0PUP2dfG/jD4LeG774j/CvUNG1Sx1G9u5fGng+a9/0XULuKb97NFL/AMueof8ALGbzYpYZv3Xnf89ofjeIuCaWYXqpH1HBnFdTB1HSkz7F/Zk/4Kg/sn/HfQbGwn+JNh4b1a7nmtYdN8bT/wBlyzTRTeTLDFLN+6vJYpv3X7mWWGvy/FZHLLKuiPuYYypjoN8x2/7Yf7Gnw1/bT+Glh4R8cXl9p9/pl9/aXhDxfp8MRl0y78ryvN/ffupopfNMUsP/AC183/nr5U0Xm5pgpY2i4Nbq39fPU9rIOIcVkmJU4PVW/P8Aq3b77/DXiL/gjV+3Npepf2f4X8UfCvxFbRDyheXms6ro8v8A11+y/wBnXf8A6Nr4ar4e4enJyd12sr/fqj98wnjnmVGko8nTujdsP+CW/wAG/g9dReJv+Cg37YHgzRNKm8mKDwXpOpRaPDqkv/PGW/vD500X/TK0ihlr2sq4PoU17yPkeIfFnOMzbjGNr/1t/Xz2Po/4gft3XPhq7b4L/sa/sX+OPif4k0rwhLrNnoNro3/COaXp+nxfuovNl1HyZYfO8oxWn+iy+d5Mvk/6mav0PBZZFytY/I5Y918Y6kn/AMP/AF/Vj4c8a+Nz/wAFK9A0yf8Aab+JFtr1lL8QNOtb3QbP/QNK8H2n9ow/a/8ARLzzv9LihtbrzptQ82aH97/qYf3NfaYTKKKhzHwc8yqvPHB7f8A840CHWPGF5bfsj2/h/Wdej8b+LdP/AOFYzeKtMill8S6Ha6jDd+ddRf6mGX7Ja+bNDL/z2879z/qYfpstxShS5T53MMI5Yi57n8OfhVqH/BPj9qGyv/8AhINC+J9tp/gXVrXRbMTyyy+GtWu7vTv9DuvO/wCPyKKG1l8mb/Xf8sZv+e1bxbrSaldfh+P9M2dONKkrGd/wT9+APijxl/wUU8E/tUQaRdS+DrQ+JtU0W8lgitdKiu7uz+yah/ZUX+tmh866i87/AJYwzf6mab99DD8LxZioum1c+x4awvLDY/Rz4ta5bz6xHp4/5dIP303nV+MylzYn5n3mFahdHwB+wf8AsW6t/wAFS9O1X43eP/GGs2Hwn17xRqGsLd6ZDDFL4rmlvJZorSKKeKWH+z7SGWK1mHlfvpYDaS/6mav2nLcXKjhUo9j89zbCKriLn2/4w/ZX1nw5qX9j6V+1h8VYraGCGWE/YvD/AO6/8pFeTiKUsZXbbNqcY0KNkeS6xqvxI0rwR4k8LwfGDVLq9074t6H4csvFU1lp/wBr+yXd5pEMv/Lp5X/L/L/yyrnjQs7FnqPhv9l7xTquvxadP+1h8S5Y5f3vneT4ei/9xFdEaOgH0l8Mf+Rb/wC29dZodDQAVpMDnfip/wAi5/23rnmNOx8y/H7/AJK18Kf9Iii/4qfVvOmm/wCWX/Eou6xWFpR3ZU5djyrTfgtrGq/Gb4o/HD4O2/8AxWOk+J9Otb3TZpooovEuk/2Fp3/EuupZv3P/AC1lmtJv+WM03/PGaavLxdCm9jsw2LjT0bPoL4B/HXwr8VvD9vf6XODEZvssIngmiurW7i/czWcvnfvYZYpvN/6418Zi6lWFS578qdOpDQ+fv+CpP/BNXUv2ofCmr/Eb4L2NlH4x1DTItH8ZaZNZ/ufFOicZtP8AXQ+TdxeZL9km82GH99LDN5Pm/a4fueGc7jh4Wkzwcbgbt2Pia7+Af7UHjHxvfW3wC8L2Pje28S+E4bXVNe+H0s1zL4atNK1G7+1w39heWkM2m6tF/aH/ACCfKmm87/ljN5M1fe0eIKc3Y+Hq5TU100OT13W7r4Ezav8AsoeDdFOha/4rvLSbwn4b1iyu4ru0l/1OoTTWs3+l+TFFFFdzf89v9Lmr2qWbU5x1Z5ssompXSPoD9mz9iLxt+1z4o1v4A/B/T7Dwv8N9Jg0n/hJ/G2jzRXUOn3f2PyprO1i/5a6hLDFa3c3/ADxmvPOm87zvJm8THYulUTuj1cLhalN7s9//AOCWP7F//BNPwp8Vv2hfgN8Dvhz9oT4deNdO0qHWNQ1mWab7JFpsUM3ky+b+5xq0WtRS+UIv30H/AExh8r5LFUXUnoj6TDvkS1Pafi3/AME4fBnhbxFdfFP4LeCNK8RC8txF4l+GvjqWW/0vUYsEk6fLMT/ZF3jsP9EmwfNijlm+2RRUwkZUuY2hipyzRTOGbwl8DPjj4c/4Zv8A2LfghpngHxbpfinRdU8ZagPBEOjnwFeafqVpqNqL+KOL/TLuU2sfkwxHybuGXzfO8mWGWXy8NSjVrWR34mFSji/bPVP+n/XQ+ufgb8D/AAR8C/C914d8Gi5uLnUb83/iDxDqU/m3+tah0lu7yfH72bEaxgDEUMUMUMMUUMUUQ99TsrHluN3c+a/AH7E37B/7ZHiP46+OfiD8BvCfimfVfjNf21zq0umeXqGl3VppGnaTdwRX8OJoT5tpN5vlSjmWWtI15p7kexje559p37KnijwLP8atY+Gf7Tx8E/D3wfezf2n4q8R+CotU1rzYtO+16h9l1XzYcafD9q8r/VSzedDd+bNXXPHewqKbOKrljruyPNf2UP2BtR+Os8XxQ/aR1e5i+E0U8V9ouj6nY/2ZrXi+HyYpv+JrF5v+h2kMv7qWKKWX7X5P/LG0/cy+dnvGEJUOSLOnC8OSc02j7L1f4mafBZW2j+DvD8VrZWkP2WHybLyorSGL/nlF/wBcf+eVfluOzF5lKyZ99RyynhYI8N+Jmo337R8mt/s0/Bi61PXdf1a9Gi+M9Y0M4h8IWE37m/u7q7/1UOoRWs0ssNp/rppvK/c+V500XsZNkCqe+zhxlanBOzPtrwB4K8K/D/wtpnw98F6BY6TpGh2cNjpmkaVCI7XT7WKLyoYYohxDF5VfaRlOK5bHzLlGbON+J/8AyOEtV7zE6KlqfH3jX/mcv+zjvCf/AKWeHaRjW0Prj4d/8jvptAUdTs/hj/yLf/beug0OhoAKuTQWZzvxU/5Fz/tvWEtdgPlz9pDVdP8ADnxI+GfiHVdYtbCxtNa1aW9vLy9iiiii/si7/wBbLN/qazeCxE3oZOoktWfPvhv/AIKP/CfwB4w+JH/CpPC+qfEH+1vE9pdaLqWg+Va6LND/AGRaQ+d/as3+ui861lh/0T7XXp4ThytiGm0eHjMaqTumeeaD+1D+0hY/GfUvjxqvg/Qfs13Zf8VP4D8K2XlS6hDF/wAvn2qab99q0X/PbyrTzof3M3+ptJoVxBwjTo0rpHflXEcq01Fs++vgn8ffBHxT8Fab4x8N+IbbVdJ1ayhurLV/P/dXUX/PH/8Ae/vv+etfkuJjVwNXlSPv8M6eIhe5m/En9i39nj4p/Gy1/aQ1rwxdWHjGK0/su+17wtezaZqGoWn/ADxlu4f3w8o/vvOilim/c/63yZpoZfaoYqpC12efVwtM4P8Aam/Zr/aK8XeFLbQrv4gQ/FnwRpOqNd6r4J13w/p48SahFnJtLDVJrSaH/Vf6qKaKKab91/xMYf8AXV7dDN5RVuY86eEjukdz+zfYfDn9jjwv4CsPgbrt9efAP4gzQx6HcarrV1fXPh3WtQlMsUst1qUpmltNQnm8rEp86G8mhiEZ+1kWv0NGTqq+55dWPs9bHwB/wSS+OviH4S/th6B458e3Rhj+KOt6t4d8dRbsRQ6tqF3/AGhazS+s39oedaf9xevbll7lh5TS2VzyZ47kna5+nP7d/wC07r37K/wavtZ+F3gM+L/iBqWlahJ4L8HwnBvZra0aeW6lxgrbQxJmU9TmKGLM00MUvyGKxTo5fOT6XPr8mwKxVaLfl+J+R37LvjD9pT4MftX6D8Z/2dfHr+J/iP8AEHxNaWPiW18U3YitfG8V1L5spvvJ/wBT5MPnXcU0X/Hp5XkxQ+V50Mv5Jw/xViK2czpSjo3226f8P3666n77xNwdgqPCMcSmuZK/S/3H7I+Gf2sPhVqP7P3iH9o7X3vfDmmeD9Pv7nxrp+vIIb/w9NaQmW7tbqLJ8qWMDPBMUoIliMsUsUsn7dGipJeZ/NM8QoyaufL3/BvF4i8e+Kf2WPiT4s+JujQ2uoeIvjdquu3sUc/m/wCmX+nadeX4/wDAya6qpUFESxFztvFkNqf+CXfxUXWjH9jv/EHjw64Jv+eE3ijUvtX/AJCklrxsY5Tw0mezg5xc0zzj9rb/AIKDfAj4C6pfaJ8RfGV74i8SeQZofh94Ls/7T1qXzYcxf6LD/qYv+mt35UX/AE1ir4rBZZiMxxTjJOx7csfSoQPnnVv25fFXxPSZdZ+CfimfTiMaX4Rg8QQ6FYXX/X/rUPnahMf9V+5tLS0/5aw+beV+g5V4bT51Jo+SzPi2UVZM2x+3n+1xB4QtvAHwl1HwR8IfB1pZfZdF8N/DHwjD9r0//pj5upedaf8AkpFX3uH4SWEgkz4mvxPWqSNX4ef8FEf23fgdrtxp+r+OtN+Kmk6bcyoNO8Z20en6h5Q6eVqFlF+6HtNaTS/9NaMTw5GnFtEYfO6jlqe3+Gv+Cq37M/xT1eIfE64v/hrqcvk/6H478qK0mm87/llfwzfZP+uPmyxTTf8APGvnMRgJUtLH0eGzNSS1OS8YTmf/AITK4z+6/wCGj/Cfk/v/ADf3P2zw7XiyjJPVHpVZRktGfXvw8/5HbTam6LopnZ/DH/kW/wDtvV3nHc6qdOxvf+0v3tUqbqbM5cRUcGeR/tCftz/st/su3Z0P43/GOxsdUkhM0PhbToJtQ1maHJxLFYWYlujF6y+V5QwM+V1PXQymc37uv9f1c5a2YezifGvx2/4K5fHH4p2kvh/9nv4L2ngjTPO48U/EEfb9Qli/1X7qws5vJh/66y3X/bGvew+RTdrnh187lFnyt42guPibrFl4w/aM+JGqeN9W0/8Ae6ZeeMJ/NtNKl/57Wtr+5tLOX/ptFFFX1WEyWth7NtfgfOYvMcXXVlcu6DPqHiMf2f4O8D69r3kz/wCu02yll8qvUk50luvwPMjSxs3ezPUfhB+y/wDtP+I/FObj4UX9hpkul6jEZ7zyvN82Wzmhi/df63/Wy1zV8fkVaDUo/idUMBjaUrpM0fCv/BOL9t3Q7y+1nwBqWu+Db27mEv2zw34h8qKWX/lr5unzQzWk3/baKvjcywWQ4htqCPpsvzPG4VWdz2Twp8Mv+CpHgeGX+29Z+F/im2im8qGHWL270HUJf+uuoQ+dD/360+Gvg8ZwxKsrwhofV0eIH1H/ABD/AG2Pi9+z7oEnjD4q/CaKW10+CWXWpvBPxO8P6p9khi/1s3+mXdnNN/2ytPOrxlwriKb5uRns0+IISjZo6T9nQSfH/wCD37Rv7La+HtZ8LahZ6rLrPh7TrvSxbTaLLrVp/aMV3a5zDN/xNo7y7imilli849f3Ve/ldSdGaTjsebjMRzxbSPzFhnuPH+peP7eDWPssureOtW1TTLzTf3UunzXeozXdp9l/65ebFNFN/wBMYq/V8tx6lQtydD8zzVVXXTXc+wtc/aa+Onj39mub406Jq4vfjB8RPhz4fvviT4o8OS5s/hJ4avrAXdpp9rkA/wBoXXmS3kveHzhNNL9ktNOil/FeJc2rYCcqEab1/r+t/wBT938PcFQzPGxnWasunp5den9WPkTQP2cYfhf4D+Cn7SPwR8T+I/BtxJ4l8aRaLrXhzVJootL1fS9Ri0+1/wBAml8mbzYYtT82KWL99EZhN5vm18FjK+Kymn9acNZNdE9PXpbTT/I/X8Dl2W8RZ1UwUpvliu7Wtn00+9X/AAPev2wP2w/F37QvwK8OafrHhK/+HHj/AMbwyWHxY0+y0y7GjeOdAsBHL/aFjLKAJoftPkxS/vfOihvJrSbzfNhmr9Y4Rzh5lRTlTPwfjThfDZRiJqE72fz76/Kx69/wSZ/bp+Af7OP7Cfhb4ey3er+KvHPifxD4svtM8L+GLOOSW7Npq8sQi+13UsWnwXX2T7LKYZbqI/19bHy9nW+A+Rwrm6dkdz4T/bA/Z8XwR8V/2Zf2vrbWPBGh+Pb/AMQ3OhrD4e1S/tZ9I1aDzbqOW7htPKhuxd3N9L5XpNF5Us372lVwM529w6KOPlFM8ki+E/gv9p7xJpvjH4BeN/A3hLwpoXhOw8O6BpF5Zf8ACMS6tf8A7271TVxpMo86zilmujF+9iim820lm/exSxTV7GV4aOHd3T89v8l/wTxszxtWrpFm/Z/8E4vjvrkEmoaH4n8HXX/XHX/Nr6h8QuGns39z/wAjwHl2ZS15yHw7/wAE5v2tNI8caRf69ofh+TSYtUhl1SW0vpZf3UU3my/8se9YS4jd7cv4kvK8xWvN+B5j4w/ZX/bA8HalJca58F7rVIpv+W2m+V+9/wC2X+uraOexqbwOfkxa0scTrH9oeG4fs/jHwfrOjf8ATHUrLyv/AEdW8cdSqb0x/wC2LoYng/wtB4Oh/wCLE+OL/wAJW39tWmqTaPoPlf2VLd2l3DdxTS6fN/on+utYvN8ryZpq5cdl2GxEdIG2Hx2Mpy1TPq74Ff8ABVDx14A1zTbb9p34Lw6pbxf8fvjD4en/AKZS/vpdKml82GL/AK5SzTf9Ma+bqcNRk9I/ifR4biGvTWqPp21+Nvj7UdHi/wCFdajbeF/D8JyNe1HR5r6XUP8Ar1tR/wAsf+mtfieZ8ZQoRvE/QaFDn0kjivjlYfFf47eHI/CGuftk694c0n/l9h8E6LNo0t3/ANvUP+lw/wDbGWGvnafiK4S2OiplUaiueMaD/wAE2fgf4O+02/h34sWth9rmlur3yfDEvmyzS/62aWXzv30v/TaX99XbR8XknY8yWQKpoa0P7BPw3879/wDGjzYv+W3neHrvyv8A0dXt0PF+6tHc5p8IKWrR0Gm/s2eH/h1NbXHhW4+H2qed/wAtv+EL/exf9tfO82uTH+JnEai3Fs0wvDmFbs0ekabrnxgsbOL+w/iB4SsPJ/54/D7zf/IvnV81PxK4nm92enLIsHTWxFPN+0Prs3+n/tfy2Ecv/LGz8I+VWdDxJz5y96BVLL8JV0aPL/FXwB+MPirzLfxj+1R4ouvOn/5Y/a4ov/INdk/EzPFryE18gwr2Rh/8MI6PPDF9u+MEt1J/020uWX/2tXTS8W+KJr+H+RxrhiK1JdN/Yf8AD+lT/aIPHEV1/wBdvD3m/wDkKaasMR4rcT7Kn+R0R4cSHaX+yj470/4Z2/wTX45alJ8PY4/s7eBRYCLSzYebLJ/Z80sP+lzafiWUf2f5v2Tyf3Pk+T+5rw6viFxVTldQ/I7lk0JKxxmg/wDBMv4b+DtY1bV/CmoRaXHrepzX89nZ6L5VpaTS/wDPKL/ljX0GWeKHFkYfB+R5GL4YpTmXPgj/AME+PDf7NXxGl+JvwF8XS+E7yb91ew6PZeVp+of9fVr/AKqavBxvHXEmb4j27p7eh9PlWGWUVXh4vRog0z/gnH4R0jVtK1e98YeItU03RvE13rumeFdT1LUJtF827N2ZcWH2vyhF/pUv/LKuTG8YcQ5nQ9h7NfgXln9qZfxA8RGe/n5HZ/tC/shP+19qGgWvxr+I1+NN8MzxXfh/R9H0z7La2E0UPlfuou/+f+WNdWScacVZRSb5PyOPPMsq4+ra+7vv+bOz0D4HXGk/ALQP2YJ9Y0LWfBPh+yhsLOz174f/AG/zfK/5bS+d/rpfO/fVVbxO4sxNf4PyOallFDBUbSsYug/sFafoemy6PY/HjVJbHzvNh0280W7uoov+mP76abzv+u03nTf9Nq9un4p8VNK8PyPMnkMN0Vbz/gnr4Xn/AOasRRf9MYdFl/8Aj1dMfFjiqmtIfkc74cp1HqYk3/BPTw/BN9og+IEsUn/PaHRZf/j1Yz8W+J39j8jf/VbLP5zc8K/s5/EDwRefaPDn7RHiiX/pjeQ3ctpF/wB/q5p+LXFD/wCXf5B/qvli+2d94VH7T+lQxXFx+0/rN1F/0+eGIa8//iJnFad3T/I3WTYVaJG1PefG+/mk+3+OPDF1HL/rvtfw5ik82upeLHFkV8H4j/sbC9jgfGH7K+n+MbyXUNc8P+CIpZv+W1n8PpbWX/v7DNXVR8XuMpbx/IzfDmDfRHJzf8E/PC97N/yPEv8A1xh8PXcv/o6anW8YuMaf2PyJ/wBWcKzyn4t/tG/Drw5qPh3xf+0J8VvixYal8QJpr/S9N8IazFYf2D4f87yrWWW18nzZvNi82bPlf6qL/pjFXn1cso0lebP17hrgfMuLMJKtQkvd+V3+H36637Gde/tL/swaKdCfXP20PjN4gbxLLdGTxPoTRabFplrFL5UYlsPskvmy+VFiU+V++64rzqmHwTnyX30O7C+Gmf1ak4XScVdJ9dLtX0S10T8rtHqHwe+O2u6yPD+r6F8edL+JvhTVfEt14TvtXh8G3WhapaatFpx1GISxTTfvv3I/WvIzXhSjl1PmT3Pl8dhYYKTpzjyyW6vdbtb9du3U91+3W/2OXUL4X/l/bZrWCzs/3Xm+VDD/AK2X/W+V+9r2+CeD4ZrWPg8+z+tlcG0isfEVxCCLLwvoPP8Ayxg8P2n/AMZm/wDItfti8PMNZXPzV8dYq7Gaj8QItA0q613XbLSNNsbK3e4vbyXRbOOK3iRSzyO7WgVVVQSWJAAGTSfh3g0ru1gXHOMnKyV2zi4f23v2c7mOaa3+Nnw0uEt4xJO732jkRIWVdzEQcDcyrk8ZYDvQvD7h3ujf/W7NV/y7l9z/AMhz/tX/ALNkdldamnxU+Gy29ldx2t7cNc6TCkE7iQpE7eRhHYRSkKcEiN8D5Tg/4h9w73Qf64Zo2l7OX3P/ACNj/henwyuPG0nwzt9d8HSeJIo/Mk8PomnG+RdpbcYAnmAbQTnb0GapeHvD97X1IfGuYKn7TlfL3tp95DN8d/hjbeIdS8JXGveDY9V0ayN5q+mOunC4sbYKjGaaMpuij2yId7ADDqc8ik/D3h69roX+uuYOClyuz0Ttu/Is+Dfi/wCBviNow8R/D1/BfiPTjIYxf6XbWF1CXABK74o2XIBBxnuPWnDw84feqdzOHG+Pw8+WpFp+ehl6f+0N+z7rFvqU2k+P/Ad7FoWf7YeFtMYafggHzj5B8rkgfNjkj1px4ByNJ2kjonxlmTspReu2j19CJ/2j/wBnqx0X/hLpfiD4Ah0w3i2h1M6hpgge4KmQQs/lqrOyRtlSSWRWBBXIrP8A4h3w/vdGceK8bGdo05X32dyC/wD2n/2bdO1O58LX/wATvh5b31pO1tfWMmpaWk8Ukb4MUqkBgyNxtblemB0oj4ecPQejX3jlxVj6iUnTk/OzH65+1h+zz4W1NdN8RfFD4d6ZdxpHOttd32lQOEkCSxtsYA7WXY44wQQRkGnLw9yB7yX3jjxXj5q8acn8macH7Q/wz1DxjF8P7Xxv4Wn1+4jF3Focd1YtdzIVMwlEAG9lKsXzgjac9KqPh7kEHZNXMpcWYpw53B8vfW33i65+0f4C8HahfaRrfi3wZYXOmWa3eo2+p3NtFNa27OiLNKpZdkZeRFDkAEuozkjNrw+4fW7RrT4sxlSCkot306jJv2m/Attq2j6DceMvAsd94itorjw/ZPqNuJdThl/1cluhfMyP/CyAhu2aH4fcPbXL/wBa8ZZyUXZb6PT1M+y/az/Z+1nxBF4T074ifDm91Wa6FrDpkGtWj3Ek5baIljEm4vu42gZzxWf/ABD7h29rol8X5nGPM6crd7P/ACNW0+P/AMKLjxU3gWDV/BT62sxhbRkvYDdCQdUMIffuHpjNH/EPOHr2uiHxnmChz8jt3tp+RkTfte/s66ReXOm3HxU+GdncWTsl5BLr9mrwMrbGV1MmVIb5SD0PHWk/Drh3rJfeaLi/NGk1Tl9z/wAjd8PftBfDzxd4gfwl4T8SeDNU1WOwjvn0zTryCe4W1dY2Scxo5YRsssRD42kSIQfmGWvDfh5uyaM5cZ5hCPNKLS2vbr2Og/4SO/8A+hW0r/wCqv8AiHeQoP8AXGsRQ+I9Q/6E/S5f+3KWj/iHeQMP9cq3c+Vf2tL2wtNNuNJ8GfspeIvi54m1f4a2FlqPxiOmXUNhq2nSrFLa3cUVn5uZf3UUf/LKb9zX5XmtGpyO3b+v8j+wOAp4GtXWJnifYpNtU0nro7q/Vfa2072PDdA+G3jrwHdxajZ/BHxd8S7bxJpEWkeKfDmq/DXWtM+zQxSxeVFbX5Hmw/6uP97/ANMc+VXzuHwVaVRPf/hz9VzbPsszmg8NzLDuN3Gad+bR6tWW93da9He+31VpXjFviJL8ANd8M+CfGvg+00nWb/QtM+FvjS3iEsX2DSJvN8RRSkmabyfNitPOl9ff996HE9aVfDpXsfzJxBhq1HNpwclLVO6872W79d+t7anu15mDw5Fm48of8JBd/wDLHzf+XPTq+u8K5SozPzHxGr0cLgk9zN8/v9o83/tyi/8AjNfvPsq76n46sRhmr2Mvx34P8L/EzwRrPw38c6OmoaJ4g0q403WLCS1jVbm1niaKWIlIgwDI7LkEEZ4INKVGrJNSejLp4yhSqKcNGndeqP54r74G/Cbwz+wb+1b490LwZBb6xoHxlsvDWj3yySFrbSTqSyG1APBXfbwnJ+b5Bz1rwHTorD1ZdU7L0ufoixU54/DU29JQcvnbf8TyjxrP4ouf2WvjfceNrO1t9Xk+PPgx9St7IkxRTHTPFxdVJzkA5H3u3fqMWl7Gbe/MvykddN0/rVFQ25J29LwPrf4Q6H8Cvhb/AMFl4dT8X69J4203W/2gr4eGPG3hGd7C+0bxFcXibtM1SK8tN9zCrERFYyExJLJG5JZF7IQw0MbaTvFvRrp5O55NWrOrkzsuW0FeL1TilurP/g90Tf8ABRbwp4X8df8ABT39srw14w+LVl4Jsrj4K6Cf7f1O1uprVJUuvCLxQzLawPKElkVItyxnaZAxBAIJiKdB4urFSsrKz1390WXVVHK8LKEOb35WStfad9/meu/8EnfE/gjR/wBiD9rHRPBvg3VPCvxD0XwfPdeLobHU4X0qWeTTNRezvdMiht0NorqjZj3MAI4mVhnA1w0cM8PUvpJL5bO1jgzmS+vYVz96MnZd91dPufI3ws+F/wAAvDn7Iuk/ErRfjSNH+IGufs0+KV1XwBaeDJSut2w1vWUF/NqSyCMOoghQRujNttIwCAV28saVD2Clze9yvS3m+p7dWtVli3CULxVSNnfZ8sdLb9fxM/8AZB/Zz0P4x/AX9onwXqiQ6Tr1j+z/AKR4t0PTbFA1rOlg1teNevKzjZcvGrRFNmMXkp3jHKoUYVKdRN2aimisZi40K9CW6c3H77q3p/kT/F74L+IvEnwW/ZN+Jt74S0/xb4z+PXxi8XeItU0e8vFhi1a5utT0a1isZJiR5cchi5LH5DcOcjmidFeypSWrk3dfNWJo4mjCtiaafLGlGKv2SUnf5foer/GT/gm14Y/Zz8afsKfA79obwHpV54r8YeMNR0z4ntaarLPFqVp/a9ibW1aQMABFa3Xlfu9ozuwWwGreeEp0pUIz3bfN96/Q5KGaxxVPF1aMnyxSa8tHd/Nq554un2eh/t6XninS7cRa1pn7c1rpen6lnN1DZJfzotsJDl/KCxxrsztwoGKxcIKu/wDHb5XOrmhLAcr+F0W7dNtzf/4OGPFfivwx/wAFLvE8/hd5hBffC/T7HWlhTKNaSgqRJgY2+b5JBP8AGEGc4FPMYwp4lqG1jLh6NGplsbbcza9f6ueMftDSG+07x34x1IpJrHh/wR8Ll8P6jJH+/wBPH9h2fED4zGCACdpGcZ561lUULSfVKNvuVzsw1k4RWzdS/n7z3Pv79mL9lP8AZ9g/4OK/ib4QHw2tV0/wj8P7TxZ4etonk/0PWmOizNdjPLMZLu4JDAr+8IxgAV6NKhhP7SlF/Cldeun/AATwMVmE/wDVynUb+KTi/Ne8rfgfIH7eulWMv/BVH4r+KNeH9n6Vp3xu8OjUPE1jbiTUNLDrIQbeHdGr7thZgWXBiTgnkcNeNNYuVvhutT2MBUi8qpqPWErLo/UvWXwE1r4vaL+3L4ksvhDpV7BomuaxeHxq+oMt9pr2usi+a1jtwQHilitZGd9uU8teRmjlhL22nez+ZDxdKhLBxcmnJKy6O6te/lc+nf8Ag3A1SL4w/tHfFz4/T/NcaR8N/BnhrzGt9xJWwSCTHyH+LS1/Tr1rqy10JVJSn2S/D/gHmcSzp4bDUqUlvKb/ABv/AO3H69Q33+fsX/2mvY9lgu58ZaBJ9u9//JL/AO00/Y4LuFoHyj8dPAegeIvCun/AuX43/D/wvc/C/wCKWtSWXhb4peLbrS/N0SWaKbT4os/vZovJNfy1VxUKseWbP7J4C4ieQUpuS1aS6dL66+pwPjT9n/4a67pEuh6L8Tf2TfD97deV5Orad8YNSlltf33nf6qUeV/+9q6NDK5q7kk/Vn3OF46lVrzcnKSs9LQ7eST6/h9/1f8AspWmkeLPiNqWv6L4q0zxLb+A/hn4V8JaL4j069F1p/8AaAtZpdQitZh/rs/6IZZev7qKvz/jDM6dR2g9j8zr1PbSlfq2/wAf13PYte8K2/iPTZNHvriW18m983zvO/1Xmww/63/pl+6ir6Tw94po5fZSZ+eZ/k0sXfqeeXnhXxhZXkun33h+/luYv9dNDZS+V/2y/wCmVf0fheL8taV5H49V4axfM7Ij/wCEc8T/APQr6z/4BS111OI8uraqZyy4bxiex8/ah/wSi/ZJvPhz4w+E9x+zdqraB488Rpr3iqx/tXVh9t1BJDIs2/7RvjwxJ2oVXnpWCzHCODi2rN3ep6yhxEqsKifvQVlotF9xhap/wRh/YW8Q6Fr/AIa1f9lfVZbLxR4gtNb1uD+3daX7RfWsd3HBLkXIKbUvrobVIU+bkglVI0/tDLnFp21d3r2v5+bNYy4mjKMlLWKaXux2dr9PJHTWf/BLX9kux/aIP7VFv+zLdDxodbk1oXzzag1uupyNue+FqZTAJy2G3hM7gGGGG6j+28oVX2nLr6vcxdPiF4X6vd8lrbK9u17Xt8yx8Qv+CZf7MPxP+JfjX4veP/2cb3Vdf+ImgRaL4wu7m51LZf2URtGjj8oTCOIq1jasHjVXBhBDZJJJZ5lM5OTjq9HqxUqPEFGjClBtRg7rRaPXy83uan7On/BP/wCBH7KfhbXfCHwU+Al3YWfihw3iU39teapLqmFZAk8ly8jOgV3UITtAduMsxM088yukmox38ysVhM7xs4yq3bjtpa3pY4fwR/wRn/Yi+H1t4k07wv8AstahBH4q0WfR9Ujl1PVJTHp8ziSW2ty8pNsjOCx8oq2WYZwcV0U8wymCesddPi/4OhFTEcTVXFyUvdd17q3XV6a/M2Ph/wD8Eqv2R/hNe+I28EfADV9Pm8VfD5vB/iBTrmqyG40KSKGA2+JJj5YKxwqJU2yZIw2WObjmWTQvdrVW0l0+8zqVOIq6ipRb5Zcy91fFvfbz9C9D/wAEvv2X20n4WaRF8AdYa1+CmqvffDVBquqH+x7qW6hui2fNzPmaCJws28fLgDBIJ/amQ+6uZe7tr/wRN8QqVVuLvVVpe6tdLdtNH0sdZ8Z/2M/hj8f/AIieBPi98WvhVq2qa98ONQk1TwTqP2q+g+wTl4ZXlCRMqTDdaxEiQOo8s8YLZueb5HOSlKSuttTKhhc9wtKdOnTkozVpe7ute683scfd/wDBKv8AZfm/aRb9rGX9mi9/4TmDVk1eXUg9+IV1D76XrW27yPP53CQpnJ3/AHsNUf2pkPtOfmV/U15uIlhPq3LLkta3L07XtexJ8bv+CZX7N37QvjbxD8RvjR+z5qmt6z4q8OW+g65dzXmpRefYQ3UF1FEoilRYys1tC29ArnaVLFWYHkr59k3tGuW+lr3+fQ3wtLP8PQjGleKi20rLR6rquze5geJv+CQP7F3jDxpoHj/xH+yrcXOpeG9N0+wsWe41Ly5oLGFILNbiMTbLoxRxogaUMxCgMWAArN59k0pJuG3m+gRfElOEoRk7Sbey66u2ml/I9D8PfsXfC7wr+0lrv7XOhfB3VIPiD4l0VNJ1rXvNv2FxZqLcLH5DSGFMfZYPmVA3ydeWz0LP8jVR1OZXfmYSwOdTwkcM/gi7pWW+vW1+rPPvib/wSI/Y5+MPjDxD49+If7NGrX2reKtattW127XWdYh+03lukiRSbY7hVTasr/KoCnOSDgYiWdZBNtuS182dVFcR4enGEHZRTS0Wz36eQzSP+CQH7HOg/ELxP8VNE/Zj1SPXfGVjq1n4kvG1bV3F5BqSSR3qGNrgogkWVxlFBXd8u3Aqf7VyJNvmWvmZyqcRypRpt6Rs1otOXbp0Ox/ZW/4J+fBb9ijTdZ0j9mf4Fan4bg8QTwzauv2nUbs3DxK6xndcyyFQA78KQPmNFPO8jo3UZLXzOfG0c8zCUXiPettol+SR6x/wivjj/oV9U/8ABXLLXTHPMmf20cn9kZj/ACsT/hFfGH/Lfwvqn/gllrpjnmTfzoP7IzH+VnofjTxZcfBiC5g/aS8LXd1ZaT+9g8YadY+Zay2n/TX/AJZeb/0yr+fsfw/WqR90/oF5jTlLliZ2pfHD4D2M1tb6t4X1m1/tC9itbKa88MeV9rml/wCWMVfNT4PzWcrxkzpWYLBx5k9zXs/jT4H86K30rwP48/7Y+BJawr8DV8Z8RcsfZXuSal8TfB/kyf8AFtviNayf8sZv+ESlii/7a0qPAeJwnw3MJYyNTcxJvjF4P0r7Nb31x4ytZLufytLh/sW7i83/AJbfuvO/65UqmV5tQejZlJ4Pqkc3r37Sfwv0O8/4qr4geI7D/TfssFneebFLLd+T53k/9dfJ/fV14bC53JWXN9zOWc8DF3aQf8NUfBeD/R/+FsapdS+R/rvP82Ktp5LxmtU2UsdlfZGvoPx38H+I9A/4SDwr4g8W6zpsP/MS02yllii/781yvKuNebRsf17K+yMyH9qj4P309zo3/CyNellih82aGH/WxV6Ky3j+2kGL6/lfZGbD+178D9V8y40r4sX8v76WKbydal/5ZU/7M8QH9hh9fyrshZv2qPg/Af8AkqGvf9sdalq/7J8Qf5Ga/Xsq8gh/ao+D85/5Khr3/bbWpaf9k+IX8jH9eynyD/hqj4Qf9FQ1T/wdS0pcPeIz+wx/2lk0OiIpv2r/AIP/APRUNU/8HUtc8uHfEa/wMP7TyaXRC/8ADWHwf/6Khqn/AIOpa0/1d8Rv5GH9tZPtZEkH7V/wX87E/wAUdU/8HU1H+rviMvsMP7WyZ9EaI/a2+A/k/v8A4kaz5X+tn8ms/wCxfENfYZEswyl9iz4b/a9+A19eS6PY/GC6l+yfur3/AELzfKpf2N4gdYMweOytvZF6H9qH4H3usf2NY/GC/upP+fOz0X97/wB+qn/V/P8Aq3f0Zf17K+yDxh+0L8PvCs1t/wAJj4o8UaXLN/qf7Y0W7tfN/wCuVL+wM9XVj+vZX2RkTftX/Bef/UfEjXvM/wCu0tazyLP1HTm+5mntsp7IveG/jT4G1zwpbeKPDmoeMtU027/1N5ptldy2svlTeT5Pm/8AbKWvMq5Pn8Hq5FKplb2SLN58cPA8E32efxB4tili1SGwn/4ll3/x9yzQ+VD/ANdv3sUP/baso4DPl1Z0c2Wfyo0ofiNbz+b5Fv8AEGX/ALl/UK6I4LPu7HzZZ/Kj6j1DRrLxPpEul6lbQy2tzDL9ptriISJJ9Qa/oOpGPLsfI6nyF4x+AnhP4Y/ECL9nERW+r/DTx7aXMUPg/VbNZE0VY0R5baCXOXs5Q4HkOC0RBEMkUQihh8+aSkDbe50HwT0jxP8ACvxY3wO1XxvdeJNHTwtJrfh691aIHUNPgS7ktTZy3IO68+4GE8o8wjiUzN+8r0YQjbY0uz3dNXv9Q8Gz2F9OZFSDgmunkjy7Am7nh3x00C3k+IPwvujK26DxDqG3j/qHXdefVpU3PZEV2+ZHx58bvgDfePv2x/iL4y1z4gztZ6RfWlrouiDT08iykudIsvtVwvzcyS/ZrbJ7eUK+84fw9BxXur7kfOZ/KSp6Mp+Bv2Y7b4ofF3w58NNQ8d3lnY61qP2a8e1tVDmP0zmvo8whRhhZS5Voux4GGlJu1z2z9tNNe8GR2v7H3wp1pPC3hew0tPPOmWa+bebOnmEnmvHyenSlVvyr7jpquWqufOes/sz6zbW1j4N8EfFGTw/e65JDbwa/YaX/AKVp4khu5ZJYiZf9cI7RhFJ1imm84ZAaKT34Uqd/hX3HFTlK+rYeGv2TtN0zTIND0HxNb2NjZWiQ2ttDpJxGqdMfva9CnTpfyr7jkxE533Zq/wDDKw/6Hkf+Cs//AB2t40qSfwr7jH3/AOZ/eR/8Mrf9T0v/AIKz/wDHa6Y0qX8q+5B7/wDM/vF/4ZZP/Q9D/wAFf/22n7Kl/KvuFaX8zD/hlk/9D0P/AAV//baPY0v5V9wWl/Mw/wCGWT/0PQ/8Ff8A9to9jS/lX3HLaX8zD/hlk/8AQ9D/AMFf/wBto9jS/lX3BaX8zK8X7NE9vNFs8bx/+Co//HamtRo2+FfcXR53L4n95zfi79m67+HfiD/hbnhPx2tpqmnWVlYakY9LIGq2Es0kPkTfvfvICSkg5UNJFgwzTRS+LXpUk/hX3HtUlLktc7fW/wBluDWL1oH8avFLA7stzHYkP5ydJc+b1ryHRo2fur7jSLlfc+ovgb8KT+2J8CtU+Cnx41e31OXw5BDLoviKKxaK7tpyZP3oxJgn5BXh42lSjUXurc6oOUup8l2HwMe0i1PTn8ZzyR2d/wDY4Q1oo/d+d0619Xh6FB0vhX3I4sRUmnuz6B/4JreAfFPgrXtc+H7eOxdeHfEdtF4g0nS/sDRnRr253xXQjkEpJhl2RymJRGBP5sucykD4zPqNFS0ivuPq8jlJxV2dR46+HyXNh4zsX1mTMn7QHhaYyeUM7ku9Bx3/ANgV8t7Kl/KvuPYrN3Ppr4Y6XcWPimK7gv8A5vIl48oU/Z0+yCi2f//Z" />

### BAKA
```py
def baka(ba, ka):
    bakabaka = ba
    for bakabakabaka in range(ka-1):
        bakabaka = ba**bakabaka
    return bakabaka
```

With the power of hindsight, I shall refractor this function as such:

```py
def tetration(a, b):
    res = a
    for i in range(b-1):
        res = a ** res
    return res
```

WOW it really is just tetration...

### HYPERBAKA
```py
def hyperbaka(ba, ka, bakabaka):
    if bakabaka == 1:
        return ba**ka
    elif ka == 0:
        return 1
    elif bakabaka == 2 and ba == ka:
        return baka(ba, bakabaka)
    else:
        bakabakabaka = hyperbaka(ba, ka-1, bakabaka)
        return hyperbaka(ba, bakabakabaka, bakabaka-1)
```

Once again, hindsight is 20/20 and we refractor as such:

```py
def knuth_up_arrow(ba, ka, bakabaka):
    if n == 1:
        return a**b
    elif b == 0:
        return 1
    elif n == 2 and a == b:
        return tetration(a, n)
    else:
        temp = knuth_up_arrow(a, b-1, n)
        return knuth_up_arrow(a, temp, n-1)
```

Higher hyperoperations... defined with [knuth's up arrow notation](https://en.m.wikipedia.org/wiki/Knuth%27s_up-arrow_notation)

Now those $\uparrow$s in the description seems very familiar

### TRIPLEBAKA
Ok finally, the last recursive layer.

```py
def triple_baka(n):
    if n == 1:
        return hyperbaka(3, 3, 4)
    else:
        return hyperbaka(3, 3, triple_baka(n-1))
```

As usual, the power of hindsight guides us to refractor as follows:

```py
def hyper_knuth(n):
    if n == 1:
        return knuth_up_arrow(3, 3, 4)
    else:
        return knuth_up_arrow(3, 3, hyper_knuth(n-1))
```

So this is some hyper operation on the hyper operation

$$
H(n) = 3 \uparrow^{H(n-1)} 3
$$

That's pretty big. ~~that's what she said~~

## CRYPTO RANDOMS
Finally, we arrive at the cryptography portion. 

```py
bits = floor(log2(secret) + 1)

a = getPrime(bits // 2) + 1
b = getPrime(bits // 2)
x = getPrime(bits // 2)
m = getPrime(bits)

def get_next():
    global x
    x = (a * x + b) % m

print(f'{bits = }')

TRIPLE_BAKA = triple_baka(64)
for i in range(1, TRIPLE_BAKA + 1):
    get_next()
    if i <= 10:
        print(i, x)

ct = secret ^ x
print(f'{ct = }')
```

So we have a Linear Congruence Generator (LCG) and the `triple_baka(64)`-th random number is xor-ed with the secret. Well, let's start with the LCG

### LCG BREAKING
On top of the `ct` we are also given the first 10 random numbers... this means we can fully recover the LCG.

Let us re-define the following for clarity sake:

$$
\begin{aligned}
p,& b, m, x_0 \text{ is prime} \\
a &= p + 1 \\
x_i &= ax_{i-1} + b \mod m
\end{aligned}
$$

First, we need to figure out $m$, this can be found by finding values congruent to $0 \mod m$. First we define $D$ as below:

$$
\begin{aligned}
D_i &= x_{i+1} - x_i \\
D_{i+1} &= x_{i+2} - x_{i+1} \\
&= (a-1)x_{i+1} + b \mod m\\
&= (a-1)(ax_i + b) + b \mod m\\
&= (a-1)ax_i + (a-1)b + b \mod m\\
&= a(a-1)x_i + ab\mod m\\
&= a([a-1]x_i + b)\mod m\\
&= a(x_{i+1} - x_i)\mod m\\
&= aD_i\mod m\\
\end{aligned}
$$

So we see that $D_{i+1} = aD_i$, this means that we can get the following values congruent to $0 \mod m$.

$$
\begin{aligned}
D_{i + 2} D_{i} - D_{i+1}D_{i+1} &= a^2 D_iD_i - (a D_i)(a D_i) \mod m \\
&= a^2 D_iD_i - a^2 D_iD_i\mod m\\
&= 0 \mod m\\
\end{aligned}
$$

So now, we retrieve $m = \gcd(D_3D_1 - D_2^2, D_4D_2 - D_3^2, ...)$. Of course, asserting that $m$ is prime.

After finding $m$, we can easily find $a$ using the $D$ we calculated earlier:

$$
\begin{aligned}
\implies &aD_i = D_{i+1} \mod m\\
\implies &a = \frac{D_{i+1}}{D_i} \mod m
\end{aligned}
$$

With $a$ comes $b$:

$$
\begin{aligned}
&x_{i+1} = ax_i + b \mod m\\
\implies &b = x_{i+1} - ax_i \mod m
\end{aligned}
$$

Nice, now we got all parameters $a, b$ and $m$ of the LCG. Lastly, we use the fact that this is a first order recurrence relation to derive the closed form of $x$. 


$$x_n = a^nx_0 + \frac{a^n -1}{a-1}b$$

Now finally, we can proceed to calculate $x_{triple\_baka(64)}$

### LCG CYCLES
The first important note is the cyclic nature of $x_n$ with cycle length $m -1$, as shown with Fermat's Little Theorem:

$$
\begin{aligned}
x_{m-1} &= a^{m-1}x_0 + \frac{a^{m-1} -1}{a-1}b \mod m\\
 & = (1)x_0 + \frac{(1) -1}{a-1}b \mod m \\
 &= x_0 \mod m
\end{aligned}
$$

So we just need to find $triple\_baka(64) \mod m - 1$.

### MODULAR TETRATION
Let's us simplify the problem to just tetration first. How do we solve modular tetration 🤔

Recalling from RSA, $pt^e \mod m = pt^{(e \mod \phi(m))} \mod m$ where $\phi(x)$ is euler's totient function. Applying to $3 \uparrow\uparrow n$ we get:

$$
\begin{aligned}
3 \uparrow\uparrow\ n \mod m &= 3^{(3 \uparrow\uparrow\ n-1 \mod \phi(n))} \mod m \\
&= 3^{[3^{\{3 \uparrow\uparrow\ n-2 \mod \phi(\phi(n))\}} \mod \phi(m)]} \mod m \\
& ...
\end{aligned}
$$

Since $\phi(n) < n$ for all $n > 1$, eventually we will reach a point where $\phi(\phi(...\phi(n))) = 1$.

This means there is a certain value $l$ such that:

$$
3 \uparrow\uparrow\ n = 3^{3^{.^{.^{.{\{3\ \uparrow\uparrow\ n-l \mod 1\}} }}}} \mod m \\
= 3^{3^{.^{.^{.{\{0 \mod 1\}} }}}} \mod m
$$

And we can see that for all $n>l$, $3 \uparrow\uparrow n \mod m = 3 \uparrow\uparrow\ l \mod m$.

This is crucial as we can effectively reduce all values to $l$. Calculating it with SAGEMATH (/sɑːɡeɪmæθ/), we get $l = 113$ under mod $m - 1$

??? "SageMath Script"
    ```py
    prev = m - 1
    from itertools import count
    for l in count(1): 
        prev = euler_phi(prev)
        if prev == 1: break
    print(l, prev)
    ```

### MAGIC OBSERVATION
It might seem like we just took a big detour. Yes... I do admit talking a little too much about the details. But we can finally see da wae (I'm old, I know). 

We just need to see that our $triple\_baka$ crazy hyperoperation is still tetration:

$$
\begin{aligned}
triple\_baka(64) &= 3 \uparrow^{(triple\_baka(63))} 3 \\
&= 3 \uparrow^{(triple\_baka(63) - 1)} (3 \uparrow^{(triple\_baka(63))} 2) \\
&= 3 \uparrow^{(triple\_baka(63) - 2)} [3 \uparrow^{(triple\_baka(63) - 1)} \{(3 \uparrow^{(triple\_baka(63))} 2) - 1\}]\\
&\cdots \\
&= 3 \uparrow\uparrow (3 \uparrow^3 ...)\\
\end{aligned}
$$

Wow, it is  tetration to an impossibly huge number... wait a huge number. That must mean it is larger than $l$! So under mod $m - 1$, `triple_baka(64)` is just $3 \uparrow\uparrow l \mod m-1$

And just like that, we just calculate $(3 \uparrow\ l \mod m-1)$-th $x$ value of the LCG, xor with $ct$ and get the flag 🥳

## SOLVE.py

```py
# LCG values
x = [
    10275910798653121436396833379154598008161,
    2068591239728841545706452127889450693176,
    26350147429806384823786121899280661716493,
    25358475244916002220884659082517978530071,
    12563752780567442975545946639227178025296,
    19642601882956204519785723889340847589962,
    6259116168994041128833294897342371591968,
    16406333604491605091556863399044907242384,
    25867766060185127305007083226436225587634
]
ct = 8194779757417092844428719009359907728048

# Find M
D = [
    x[i] - x[i - 1] for i in range(1, len(x))
]

m = D[0] * D[2] - D[1] * D[1]
for i in range(1, len(D) - 1):
    m = gcd(D[i - 1] * D[i + 1] - D[i] * D[i], m)

assert m.is_prime(), "m not prime, try one of its prime factors"

# Convert all integers into GF(m) -> modular calculation under mod m
F = GF(m)
x = list(map(F, x))
D = list(map(F, D))

# Find A
a = D[1] * D[0] ^ -1

# Find C
c = x[1] - x[0] * a

# Find x0
x_0 = (x[0] - c) / a
print(f"Broke LCG: {a = }; {x_0 = }; {c = }; {m = }")

# Closed form
def x(n): return a ^ n * x_0 + c * (a ^ n - 1) / (a - 1)


# Find l
prev = m
from itertools import count
for l in count(1): 
    prev = euler_phi(prev)
    if prev == 1: break
print(f"[*] Found {l = }")


def tetrate(a, b, mod): # Faster Modular Tetration
    moduluses = [mod]

    # Cap when euler_phi = 1
    while moduluses[-1] != 1: moduluses.append(euler_phi(moduluses[-1]))

    res = 0
    for i in range(min(b, len(moduluses)-1), -1, -1):
        res = pow(a, res, moduluses[i])
    return res

n = tetrate(3, l, m - 1)
print(f"[*] triple_baka(64) % m - 1 = {n}")

x_n = int(x(n))
print(f"[*] x_{{triple_baka(64)}} = {x_n}")


from Crypto.Util.number import *
print(f"[*] FLAG: {long_to_bytes(x_n ^^ ct)}")
```

Flag: `SSMCTF{b4kabaka!}`
