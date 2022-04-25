# Static-S-n-f-ve-yeler
 static void Main(string[] args)
        {
            Console.WriteLine("Çalışan Sayısı{0}", Calısan.CalısanSayısı);
            Calısan calısan = new Calısan("Rabia","Çakmak","Bilişim Teknolojileri");
            Console.WriteLine("Çalışan Sayısı{0}", Calısan.CalısanSayısı);

            Console.ReadLine();
       
        }
    }
    class Calısan
    {
        private static int calısanSayısı;

        public static int CalısanSayısı { get => calısanSayısı;  }

        private string Isim;
        private string SoyIsim;
        private string Departman;
          // Static bir kurucu oluşturmak istiyorsak.
          static Calısan()
        {
            calısanSayısı = 0;// Çalışan sayımız 0.


        }


        public Calısan(string ısim, string soyIsim, string departman)
        {
            this.Isim = ısim;
            this.SoyIsim = soyIsim;
            this.Departman = departman;
            calısanSayısı++;
        }// Ben bir class oluşturdum ardından kurucusunu oluşturdum.
        

    }
}
