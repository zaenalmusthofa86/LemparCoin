# Membuat aplikasi game android sederhana lempar coin

Tampilan Menu Utama

![img](https://github.com/zaenalmusthofa86/LemparCoin/blob/main/img/1.JPG)

Penjelasan di Event OnClick

```
if (view==buttonLempar)
```
Jika buttonLempar ditekan maka tampilannya :

```
TextView tw=(TextView)findViewById(R.id.textView1);
ImageView iw=(ImageView)findViewById(R.id.imageView1);
```

Identifkasikan dan cari ID. tw dengan textView1, iw dengan imageView :

```
 if (acak.nextDouble() < 0.5) {
     tw.setText("Kepala");
     iw.setImageResource(R.drawable.head);
 }
```

Jika random next double kurang dari 0.5, maka akan muncul text “Kepala” dan gambar head.

![img](https://github.com/zaenalmusthofa86/LemparCoin/blob/main/img/2.JPG)

```
else {
   tw.setText("Cross");
   iw.setImageResource(R.drawable.tail);
 }
```

selain itu, maka akan muncul text “Cross” dan gambar tail.

```
buttonLempar.setVisibility(View.INVISIBLE);
buttonUlang.setVisibility(View.VISIBLE);
buttonKeluar.setVisibility(View.VISIBLE);
```

buttonLempar disembunyikan, buttonUlang dan buttonKeluar dimunculkan.

![img](https://github.com/zaenalmusthofa86/LemparCoin/blob/main/img/3.JPG)

```
else if (view==buttonUlang) {
```

Jika ditekan buttonRepeat maka akan muncul tampilan :

```
TextView tw=(TextView)findViewById(R.id.textView1);
ImageView iw=(ImageView)findViewById(R.id.imageView1);
```

Identifkasikan dan cari ID. tw dengan textView1, iw dengan imageView :

```
buttonLempar.setVisibility(View.VISIBLE);
buttonUlang.setVisibility(View.INVISIBLE);
buttonKeluar.setVisibility(View.INVISIBLE);
```

buttonLempar dimunculkan, buttonUlang dan buttonKeluar disembunyikan.

![img](https://github.com/zaenalmusthofa86/LemparCoin/blob/main/img/4.JPG)

```
else if (view==buttonKeluar){
```

Jika klik buttonExit :

```
this.finish();
```

Keluar aplikasi.





