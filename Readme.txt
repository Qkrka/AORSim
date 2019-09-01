AORSim_V0.3.1.2.jar - the simulator
konfiguracija.txt - configuration of the simulator
microProgram.txt - processor microcode
test/Codetest3a - test with random instructions
test/Codetest3b - merge sort test, array length - 1000h, array start address - 1010h
test/3bins - clean instructions for 3b

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

Da bi se pokrenuto simulator racunarskog sistema potrebno je da na racunaru bude instalirana java virtuelna masina verzija 1.7 ili novije.
Pokretanje simulatora se postize pomocu jar fajla koji je dat u prilogu. 
Ukoliko se prilikom pokretanja simulator ne pokrene potrebno je proveriti da li postoji instalirana java, i da li se putanja do java.exe programa nalazi u sistemskoj promenljivi PATH. Ako se ne nalazi dodati putanju do java.exe programa u promenljivu PATH (http://docs.oracle.com/javase/tutorial/essential/environment/paths.html). 

U ovoj arhivi se nalaze sledeci fajlovi:
1. jar - simulator racunarskog sistema
2. konfiguracija.txt - konfiguracioni fajl u kome se nalaze opisi Fetch1, Fetch2, Fetch3, Exec3, KMOPR1, KMADR1 i CONTRODC jedinica, kao i ostalih zajednickih promenljivih. Ucitava se automatski prilikom pokretanja simulatora.
3. microProgram.txt - nalaze se mikroinstrukcije koje procesr izvrsava i koje kao komentare ispisuje kada se izvrsava mikroinstrukcija na datoj adresi mikroprogramske memorije. Na osnovu ovog fajla se automatski kreira sadrzaj mikroprogramske memorije. Ucitava se automatski prilikom pokretanja simulatora. 
4. /src/images - direktorijum sa slikama
5. error.txt - izlazni fajl sa greskama prilikom podizanja simulatora. U slucaju da ne bude bilo gresaka prilikom pokretanja ili rada fajl bi trebalo da bude prazan.
6. Code.txt - primer sadrzaja operativne memorije. Sadrzaj operativne memorije se ne ucitava automatski vec se ucitava koristeci File -> Load memory ili Ctrl + N 
7. microProgram_V1.txt - nalaze se novija verzija programa sa mikroinstrukcijama. Ne ucitava se automatski prilikom pokretanja simulatora. Da bi se koristio potrebno je trenutnu verziju mikroprograma (microProgram.txt) sacuvati, a dati microProgram_V1.txt preimenovati u microProgram.txt.

Racunarski sistem koji se simulira: dr Jovan Djordjevic <jdjordjevic@etf.bg.ac.rs>
Implementacija osnovne varijante resenja simulatora racunarskog sistema u programskom jeziku Java: Aleksandar Milic <mrevil1990@yahoo.com>
Transformacija simulatora u konfigurabilni simulator arhitekture i organizacije racunara: dr Zaharije Radivojevic <zaki@etf.bg.ac.rs>

Greske u radu simulatora i sugestije slati na adresu: zaki@etf.bg.ac.rs
