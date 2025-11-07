Soru1 --> Genericler (Generics) --> Fonksiyonlara esneklik katmak ve farklı veri tipleriyle güvenli bir şekilde çalışmak için kullanılan Generic tipleri ($<T, U>$) gösterir. İki farklı tipteki diziyi birleştirir.

Soru2 --> Union Tipleri ve Type Guard (Tip Koruması) --> Bir değişkenin birden fazla tipe sahip olabileceği Union tipleri

Soru3 --> Sınıflar (Classes) ve Kapsülleme (Encapsulation) --> logHistory değişkenini private anahtar kelimesi ile tanımlayarak sınıf dışından erişimi kısıtlar ve kapsülleme ilkesini uygular. Bir sınıfın temel yapısını ve metotlarını gösterir.

Soru4 --> Keyof ve Indexed Access Tipleri ile Genericler --> Bir nesnenin anahtar (key) tiplerini kısıtlamak için K extends keyof T kısıtlamasını ve bir anahtar aracılığıyla nesnenin değer tipine erişmek için Indexed Access Tipleri (T[K]) kullanır. Güvenli özellik erişimini sağlar.

Soru5 --> Fonksiyon Aşırı Yüklemesi (Function Overloading) --> Aynı isimde birden fazla fonksiyon imzası tanımlayarak (yalnızca parametre sayısına/tipine göre) bir fonksiyonun farklı girdilere göre farklı dönüş tiplerine sahip olmasını sağlar.

Soru6 --> Generic Sınıflar ve Map Kullanımı --> Bir sınıfın (Cache) depolayacağı anahtar (K) ve değer (V) tiplerini dinamik olarak belirlemek için Generic kullanır. Veri saklama için standart bir JavaScript veri yapısı olan Map'in tip güvenli kullanımını gösterir.

Soru7 --> Utility Tipleri (Partial, Readonly) ve İmmutability --> Mevcut bir tipin tüm alanlarını opsiyonel yapan Partial<T> ve tüm alanlarını salt okunur yapan Readonly<T> hazır Utility Tiplerini kullanır. Object.freeze() ile birlikte değişmezlik (immutability) kavramını vurgular.

Soru8 --> Rest Parametreler (Rest Parameters) --> Bir fonksiyona sınırsız sayıda argüman geçilmesini sağlayan ve bu argümanları bir dizi olarak yakalayan Rest Parametreler (...numbers: number[]) kullanımını gösterir.

Soru9 --> Soyut Sınıflar (Abstract Classes) --> Doğrudan örneği oluşturulamayan ve alt sınıfların uygulamak zorunda olduğu metotlar

Soru10 --> Static Üyeler (Static Members) ve Sabitler (Constants) --> Bir sınıfa ait, ancak sınıfın bir örneğine (instance) bağlı olmayan statik özellikler (static readonly PI) ve metotlar (static calculateCircumference) tanımlar. Sınıf üzerinden direkt erişim sağlanır.

Soru11 --> Conditional Tipler ve infer (Promise) --> Bir tipin Promise olup olmadığını kontrol eden ve eğer Promise ise içindeki tipini (<infer U>) çıkaran bir Koşullu Tip (UnwrapPromise<T>) kullanır.

Soru12 --> Conditional Tipler ve infer (Dönüş Tipi) --> Bir fonksiyon tipinin dönüş tipini (<infer R>) çıkaran ve bu sayede fonksiyonun döndüreceği değeri statik olarak tipleyen bir Koşullu Tip (GetReturnType<T>) kullanır.

Soru13 --> Mapped Tipler ve Key Remapping (Getter Oluşturma) --> Mevcut bir tipin her bir özelliğini, adını get ile başlatıp büyük harfe çevirerek yeniden haritalayan (Key Remapping) ve dönüş tipi orijinal özelliğin tipi olan bir getter metodu oluşturan Mapped Tip (CreateGetters<T>) kullanır.

Soru14 --> Derin Salt Okunurluk (DeepReadonly) ve Özyineleme (Recursion) --> Bir nesne tipinin yalnızca ilk seviyesini değil, iç içe geçmiş tüm alt nesnelerini ve dizi elemanlarını da özyinelemeli olarak readonly yapan ileri seviye bir Mapped Tip kullanır.

Soru15 --> Değer Tipine Göre Özellik Seçimi (PickByValueType) --> Bir tipten, yalnızca belirtilen değere (V) sahip özellikleri filtreleyen ve seçen (T[K] extends V ? K : never) dinamik bir Mapped Tip kullanır. boolean tipindeki özelliği filtreleyerek dışarıda bırakır.

Soru16 --> Nominal Tipler (Branding) --> Temelde aynı olan (örneğin string) ancak mantıksal olarak farklı olması gereken tipleri (UserID, PostID) birbirinden ayırmak için & { __brand: T } yapısını kullanarak Nominal Tiplendirme (Branding) uygular.

Soru17 --> Union Tiplerini Filtreleme (Exclude Pattern) --> Koşullu Tipleri kullanarak birleşim (Union) tipinden belirtilen alt tipleri (T extends U ? never : T) çıkaran bir mekanizma (FilterUnion<T, U>) oluşturur. TypeScript'in yerleşik Exclude Utility Tipinin mantığıdır.

Soru18 --> Fonksiyonun Son Parametresini Çıkarma (infer ile Tuple) --> Fonksiyon tipinin parametrelerini tuple olarak çıkarırken, sondan bir önceki parametreleri bir dizi (...infer R) ve son parametreyi (infer L) yakalamak için infer anahtar kelimesini kullanan ileri seviye bir Koşullu Tip kullanır.

Soru19 --> Diziyi Düzleştirme (Flatten) --> Bir tipin dizi olup olmadığını kontrol eden ve eğer dizi ise eleman tipini (infer ElementType) çıkaran, değilse tipi olduğu gibi bırakan basit bir Koşullu Tip (Flatten<T>) kullanır.

Soru20 --> Template Literal Tiplerle Route Parametrelerini Çözümleme --> Template Literal Tipleri ve Özyinelemeli Koşullu Tipleri kullanarak, bir URL rotası dizesindeki (/users/:id) dinamik parametre adlarını (:id) ayrıştırıp, tip olarak karşılık gelen bir nesne ({ id: string }) oluşturan karmaşık bir tip (ParseRouteParams<T>) kullanır.







