# Social_Resume_Database

1.	Write a brief explanation using your own words about these applications in terms of their scope.

FACEBOOK
Facebook, insanların başka insanlarla iletişim kurmasını ve bilgi alışverişi yapmasını amaçlayan bir sosyal paylaşım sitesidir.  4 Şubat 2004 tarihinde Harvard Üniversitesi 2006 devresi öğrencisi Mark Zuckerberg tarafından kurulan Facebook, öncelikle Harvard öğrencileri için kurulmuştu. Daha sonra Boston civarındaki okulları da içine alan Facebook, iki ay içerisinde Ivy Ligi okullarının tamamını kapsadı.  İlk sene içerisinde de; Amerika Birleşik Devletleri'ndeki tüm okullar Facebook'ta mevcuttu. 
Facebook başlangıçta Amerika’da bulunan üniversite öğrencileri arasında sosyal ağ oluşturmak amacıyla kuruldu ancak insanların internet üzerinden haberleşme olanakları arttıkça insanlar birbiri hakkında daha fazla bilgi edinme ihtiyacı hissetti.Bu gereksinimlere bağlı olarak Facebook’a birçok yenilikler getirildi.Bunlardan genel olarak bahsedecek olursak; kullanıcıların eski arkadaşlarıyla iletişime geçmelerini sağlamak,tanıdık oldukları kişilerle mesajlaşmalarını sağlamak,beğendikleri şarkıları,videoları paylaşmak,çeşitli reklam uygulamalarını Facebook üzerinden ücretsiz yayınlamak(satılık ev ilanları,kiralık ev ilanları,iş ilanları…),arkadaşlarının doğum günlerini kutlamak ve onlara Facebook hediyeleri göndermek,Facebook durum bilgisi ile kullanıcıların arkadaşlarını, Facebook gruplarını, mevcut durumları ve eylemleri hakkında bilgilendirmek,yazılım geliştiricilerin kısıtlıda olsa bazı uygulamalar geliştirmesine olanak sağlamak olarak sıralayabiliriz.

LINKEDIN
           Linkedin çalışanlar, iş arayanlar ve işverenlerin profesyonel anlamda kullanımı amacıyla tasarlanmış bir sosyal ağ sitesidir. 2003 yılında kurulmuş olan Linkedin, 200 ülkede 135 milyondan fazla kullanıcısı olan bir ağ. LinkedIn’in bu kadar hızlı büyümesinin en önemli nedeni dünya genelindeki profesyonellere gerçek ve etkili bir iletişim ağı kurma, network geliştirme imkanı vermesidir. Türkiye’de de 1 milyona yaklaşan hatırı sayılır bir kitlesi var.
	Linkedin vasıtasıyla iş başvuruları yapabilir,yapmış olduğumuz sunumları ve okuduğumuz kitapları paylaşabilir, kişisel blog reklamı yapabilir,bağlantımız olmayan kişilerle mesajlaşabilir,nitelikli arama filtreleri oluşturabilir ve otomatik arama sonuçları gönderilebilir,ilgimizi çeken alanlar ile ilgili gruplara dahil olabilir,bilgi ve görüş alışverişi amacıyla soru sorup konunun uzmanlarından cevaplar edinebilir veya benzer şekilde bize soru sorulduğunda soruları cevaplayarak bilgi ve tecrübelerimizi gösterebilir ve bu şekilde puanımızı artırarak sektörde insanların dikkatini çekebiliriz.
            Linkedin’de aynen Facebook’ta olduğu gibi arkadaş edinebilir ve aynı zamanda meslektaşlarımızla bağlantı kurup iletişime geçebiliriz.Linkedin bize iş hayatına yönelik fırsatlar sunar ve kariyer amaçlı kullanılır.
	





2.	Write an analysis report for each of the database model/application


a.	What is the aim of each application?
          Facebook, insanların başka insanlarla iletişim kurmasını ve bilgi alışverişi yapmasını amaçlayan bir sosyal paylaşım sitesidir.  Facebook; insanları arkadaşlarına, çalışan, eğitim gören ve yaşadıkları ortamda yer alan diğer insanlara bağlayan sosyal bir araçtır. İnsanlar, Facebook'u kullanarak arkadaşlarıyla iletişim sağlayabilir, sınırsız miktarda fotoğraf yükleyebilir, link ve videoları paylaşabilir ve tanıştıkları insanlar hakkında daha fazla bilgi alabilirler. 
      Linkedin çalışanlar, iş arayanlar ve işverenlerin profesyonel anlamda kullanımı amacıyla tasarlanmış bir sosyal ağ sitesidir.


b.	What are the main entities of them?

	USER
	PROFILE
	CONNECTION
	MESSAGE
	STATUS
	FRIEND
	FEED
	FEED_INFO
	ORGANIZATION
	LANGUAGE
	USER_PROFILE
	NOTIFICATION
	THUMB_UP_DOWN
	BOOKMARK
	CV

c.	What are the characteristics of each entity?
  
•	    USER TABLOSU:Bu tablonun attribute’leri;
       user_id
       token
       user_name
       password
       name_first
       name_middle
       name_last
       email_address
       picture
       active
       online
       gender
       current_organization_id
       created_at

USER tablosu temel tablodur.Amacımız sosyal bir ağ ortamı oluşturmak olduğu için      temelde bir kullanıcı olmalıdır.Bu kullanıcıya ait isim,şifre gibi temel unsurlar olmak üzere kullanıcının tanınabileceği belli ögeler olmalıdır.


•	PROFILE TABLOSU:Tablonun attribute’leri; 
profile_id
user_id
privacy
dob
about_me
relationship
phone
interests
education
hobbies
fav_movies
fav_artists
fav_books
fav_animals
religion	
	
PROFILE tablosuda temel tablolardan biridir.Her kullanıcının belli başlı bilgilerini paylaşmasını sağlayan tablodur.Kullanıcıya ait id,kimlerle arkadaş,nerede eğitim görmüş,hobileri,sevdiği kitaplar,filmler,sporlar gibi bilgilerin tutulduğu tablodur.




•	ADDRESS TABLOSU:Tablonun attribute’leri;
address_id
city_id
profile_id
address
privacy
zip_or_postcode

                          ADRESS tablosunda kullanıcıya ait adres bilgileri tutulur.Kullanıcının hangi    şehirde,hangi ülkede olduğu o şehre ait posta kodu bilgisi gibi  ögeler tutulur.


•	 CITY TABLOSU:Tablonun attribute’leri;
      city_id
      country_id
      city
	
CITY tablosunda kullanıcının hangi şehirde bulunduğu ve bu şehrin hangi ülkede olduğuna dair bilgiler yer alır.	


•	 COUNTRY TABLOSU:Tablonun attribute’leri;
      country_id
      country

      COUNTRY tablosunda kullanıcının hangi ülkede bulunduğuna dair bilgiler yer alır.
  
  
•	CONNECTION TABLOSU:Tablonun attribute’leri;
      connection_id
      connection_user_id
      user_id
      created_at	

      CONNECTION tablosukullanıcının kimlerle bağlantı kurduğunu      
      göstermeye yarayan tablodur.


•	MESSAGE TABLOSU:Tablonun attribute’leri;	
      message_id
      message
      created_at
      is_read
      is_spam
      to_who
      is_reply
      user_id

      MESSAGE tablosunda	kullanıcının bir mesajı yaratma zamanı,bu mesajı kime gönderdiği ve mesajın diğer kullanıcı tarafından okunup okunmadığına dair bilgiler yer alıyor.


•	STATUS TABLOSU: Tablonun attribute’leri;
      status_id
      message
      created_at	
      thumbs_up
      thumbs_down
      privacy
      is_reply	

      STATUS tablosundakullanıcının durum bilgisi,bu durumun ne zaman oluşturulduğu,durumun beğenilip beğenilmemesi ve kullanıcının durumunun kimlere açık olduğunu gösteren privacy bilgileri tutuluyor.


•	COMMENT TABLOSU:Tablonun attribute’leri;
      comment_id
      message	
      created_at
      status_id
      friend_id	

      COMMENT tablosundakullanıcının arkadaşlarının,hangi duruma hangi yorumları yazdığına dair bilgiler tutulur.


•	 THUMB_UP_DOWN  TABLOSU: Tablonun attribute’leri;
       thumb_up_down_id
       flag,created_at
       status_id	
       friend_id

     THUMB_UP_DOWN  tablosunda kullanıcının hangi arkadaşının,hangi  durumu beğenip  beğenmediğini gösteren bilgiler tutulur.


•	  FRIEND TABLOSU: Tablonun attribute’leri;
        friend_id
        friend_user_id
        is_subscriber	
        privacy	
        created_at
        user_id
        friend_list_id	

        FRIEND  tablosunda kullanıcının arkadaşlarının bilgilerinin yer aldığı ögeler tutulur.Kullanıcı kiminle ne zaman arkadaş oldu,arkadaş listesinde kimlerin olduğu ve bu bilginin gizlilik bilgisi tutulur.


•	FRIEND_LIST  TABLOSU: Tablonun attribute’leri;
friend_list_id
list_name
privacy	

FRIEND_LIST tablosunda arkadaş listesinde kimler var ve bunu kimler görebilir bilgileri yer alıyor.


•	BOOKMARK TABLOSU:Tablonun attribute’leri;
 bookmark_id
 url
 rating
 privacy
 created_at
 bookmark_category_id
 bookmark_sub_category_id	

BOOKMARK  tablosunda  Facebook sayfasının sol tarafında yer alan gruplar,uygulamalar,ilgi alanları gibi bilgiler yer alır.Bu sayede kullanıcı hangi gruplara üye,hangi uygulamaları kullanıyor,yakın arkadaşları kimler gibi bilgilere hızlı erişimi sağlar.


•	BOOKMARK_INFO TABLOSU:Tablonun attribute’leri;
bookmark_info_id 
bookmark_id
user_id
favorite
clicks
privacy

BOOKMARK_INFO tablosunda, Kullanıcının sahip olduğu bookmark  bilgilerini tutar, favori bookmarklarını belirler.


•	BOOKMARK_CATEGORY TABLOSU:Tablonun attribute’leri;
bookmark_category_id
name

                     BOOKMARK_CATEGORY tablosu gruplar,uygulamalar,sayfalar,arkadaşlar gibi temel başlıkları tutan tablodur.

•	BOOKMARK_SUB_CATEGORY TABLOSU:Tablonun attribute’leri;
 bookmark_sub_category_id
 name
 bookmark_category_id	

                             BOOKMARK_SUB_CATEGORY tablosunda her bir book kategori için özelleşmiş alt kategorileri tutar.Örnek olarak grup kategorisinin sub categorisi olarak okul,iş ve sosyal gruplar vardır.


•	FEED TABLOSU:Tablonun attribute’leri;
 feed_id
 feed_url
 rating
 privacy
 created_at
 feed_category_id

FEED tablosunda facebook veri tabanında yer alan sayfalar, resimler, videolar vs bir bütün olarak tutulur.


•	FEED_INFO TABLOSU:Tablonun attribute’leri;
 feed_info_id
 feed_id
 user_id
 favorite
 clicks 
 privacy
	
      FEED_INFO tablosunda kullanıcıya özel anasayfa bilgilerini tutan tablodur.Kullanıcı feed tablosundan seçtiği kayıtlara göre anasayfasını doldurur.


•	FEED_CATEGORY  TABLOSU:Tablonun attribute’leri;
feed_category_id
name

 FEED_CATEGORY tablosunda  fotoğraflar, videolar, gruplar, takip    edilenler, oyunlar,arkadaşlar gibi kategorilerin yer aldığı tablodur.



•	ORGANIZATION TABLOSU:Tablonun attribute’leri;
 organization_id	
 organization_name
 organization_description	

              ORGANIZATION tablosunda kullanıcının hangi organizasyonlarda yer aldığı ve bu organizasyona ait bilgiler tutulur.


•	LANGUAGE TABLOSU:Tablonun attribute’leri;
 language_id
 user_id,
 language	

LANGUAGE tablosunda kullanıcının uygulamayı hangi dilde kullandığının bilgisi yer alır.


•	USER_PROFILE  TABLOSU:Tablonun attribute’leri;
 user_profile_id
 user_id
 date_created	
 date_last_updated	

USER_PROFILE tablosunda kullanıcının profili hangi tarihte oluşturuldu,hangi tarihte güncellendi gibi bilgilerin tutulmasını sağlar.



•	NOTIFICATION  TABLOSU:Tablonun attribute’leri;
 notification_id
 msg
 type
 privacy 
 created_at
 user_id	

NOTIFICATION tablosunda bildirimin türü,kimler tarafından  görülebileceği ve ne zaman meydana geldiği gibi bilgiler tutulur.


•	CV TABLOSU:Tablonun attribute’leri;
 cv_id
 user_id
 date_created
 date_updated	

CV tablosunda kullanıcının CV bilgisini tutan cv_id ve kullanıcının CV’sini hangi tarihte oluşturduğu,hangi tarihte güncellediği bilgileri tutulur.


•	GROUPS TABLOSU:Tablonun attribute’leri;
 group_id
 created_by_user_id	
 group_name
 group_description
 group_date_started	
 group_date_ended

GROUPS tablosunda grubun içerik bilgisini tutan group_id alanı yer alır.Kullanıcı bu grubu ne zaman yarattı, grubun ismi, grubun tanımı(dışarıdan katılacak kişiler için anlaşılması için),grupta yapılan aktiviteler  ve ne zaman grup kuruldu, ne zaman sonlandırıldı bilgileri tutulur.


•	USER_GROUP TABLOSU:Tablonun attribute’leri;
user_id	
group_id
date_joined
date_left

USER_GROUP tablosunda bir grupta kimler yer alıyor,bu kişilerin gruba katılma ve gruptan ayrılma tarihleri tutuluyor.


•	PEOPLE_BEING FOLLOWED  TABLOSU:Tablonun attribute’leri;
user_id
user_being_followed_id
date_started_following
date_stop_following	

PEOPLE_BEING FOLLOWED  tablosunda kullanıcılar birbirlerini ne zaman takip etmeye başladılar,ne zaman takip etmeyi bıraktılar bilgileri tutulur.


•	PROFILE_SECTION  TABLOSU:Tablonun attribute’leri;
 profile_section_id
 user_profile_id
 profile_section_name
 profile_section_text	
 date_updated	

PROFILE_SECTION  tablosunda kullanıcının iş başvurusu için kullanacağı profilden  bahsediliyor.Kullanıcının nerelerde eğitim aldığı,hangi sertifikaya sahip olduğu  gibi kullanıcı hakkında bilgi edinilecek alanlar yer alıyor.


•	RECOMMENDATION   TABLOSU:Tablonun attribute’leri;
user_recommending_id
user_being_recommended_id
date_of_recommendation

RECOMMENDATION   tablosunda yine iş başvurularında bir kişiye referans olarak o kişiyi  bazı şirket, firma veya o alanda ilgili kişilere tavsiye etme söz konusudur.	


•	PRIVACY_TYPE  TABLOSU:Tablonun attribute’leri;
privacy_type_id
 privacy_name	

PRIVACY_TYPE   tablosunda kullanıcının bilgilerini kimlerle paylaşmak istediğinin bilgileri tutulur.Privacy alanı sadece kişiye özel olabilir,sadece arkadaşları olabilir, arkadaşlarının arkadaşları olabilir veya herkes tarafından görülüyor olabilecek  şekilde ayarlanır.

	_______________________________________________________________     	
          
•	CV_SECTION: Tablonun attribute’leri;
cv_id
cv_section_name
date_created_name
date_updated
cv_section_text

CV_SECTION tablosunda kullanıcıların oluşturdukları Cv lerin içerikleri tutulur. Bu içerikler bir başlık altında toplanmıştır (cv_section_name)


d.What relationships exists among the entities?

 	PROFILE.User_id	   USER.user_id
 	CONNECTION.user_id	               USER.user_id
 	CONNECTION.connection_user_id	               USER.user_id
 	MESSAGE.user_id	          USER.user_id
 	MESSAGE.to_who                 USER.user_id
 	STATUS.user_id	          USER.user_id
 	FRIEND.friend_user_id	                USER.user_id
 	FRIEND.user_id	                        USER.user_id
 	BOOKMARK_INFO.user_id	                USER.user_id
 	FEED_INFO.user_id	          USER.user_id
 	GROUPS. created_by_user_id	               USER.user_id
 	USER_GROUP.user_id	              USER.user_id
 	USER.current_ organization_id	                     ORGANIZATION.organization_id
 	LANGUAGE.user_id	          USER.user_id
 	PEOPLE_BEING_FOLLOWED. user_being_followed_id  		USER.user_id
 	PEOPLE_BEING_FOLLOWED. user_id		USER.user_id
 	USER_PROFILE.user_id	          	USER.user_id
 	 NOTIFICATION.user_id	         	   USER.user_id
 	RECOMMENDATION. user_being_recommended_id		USER.user_id
 	RECOMMENDATION. user_recommending_id		USER.user_id
 	CV.User_id	        USER.user_id
 	CV_SECTION. cv_id 		CV.  cv_id
 	 ADDRESS. profile_id   	   	PROFILE. profile_id   
 	ADDRESS. city_id		CITY. city_id
 	CITY. country_id	   COUNTRY. country_id
 	COMMENT. friend_id		FRIEND. friend_id
 	COMMENT. status_id		FRIEND. status_id
 	THUMB_UP_DOWN. status_id		STATUS. status_id
 	THUMB_UP_DOWN. friend_id		FRIEND. friend_id
 	FRIEND. friend_list_id		FRIEND. friend_list_id	
 	BOOKMARK. bookmark_category_id		                                           		   BOOKMARK_CATEGORY.bookmark_category_id
 	BOOKMARK. bookmark_sub_category_id		                                       		    BOOKMARK_SUB_CATEGORY.bookmark_sub_category_id
 	BOOKMARK_SUB_CATEGORY. bookmark_category_id		BOOKMARK_CATEGORY. bookmark_category_id	
 	BOOKMARK_INFO. bookmark_id	    BOOKMARK. bookmark_id
 	FEED_INFO. feed_id		FEED.  feed_id
 	FEED. feed_category_id	  FEED_CATEGORY. feed_category_id
 	USER_GROUP. group_id 	    GROUPS. group_id
 	PROFILE_SECTION. user_profile_id	        USER_PROFILE. user_profile_id


e.What are the constraints related to entities, their characteristics and the
relationships among them?

Tasarladığımız veritabanımızda Primary Key,Foreign Key ve Check Constraint türleri bulunmaktadir. Primary Key Constraint, Primary Key olan sahalara aynı değer  girilmesini  ve sahaların  NULL olmasını engeller. Bizim tasarımımızda Primary Key sahaları otomatik olarak birer artmaktadır. Bu da tekrarı önler. Foreign Key, bir tablodaki bir sütuna ait verilerin başka bir tablonun belirli bir sütunundan gelmesini denetler.  Bazı tablolarımızda Primary Key e uygulanan bir değişiklik, ona bağlı olan Foreign Keyleri de etkilemiştir.  Check Constraint, belirtilen formata göre verilerin girilmesini sağlar. Bizim veritabanımızdaki Check Constraintler;password ün en az 8 karakter olması,gender in ‘F’ ya da ‘M’ olması,bir kişinin kendini arkadaş olarak eklememesi.


3.	Design the relational model of the social resume database to integrate the initial designs.
Your integration methodology should try to reuse the constructs given. You can redesign or
extend the initial designs. Write down the appropriate SQL scripts (DDL statements) for
creating the database and its relational model. You can select any of the DBMS you wish.


CREATE TABLE [ADDRESS] (

	 address_id                    int IDENTITY(1,1) NOT NULL,
	 city_id                       int NOT NULL,
	 profile_id                    varchar(50) NOT NULL,
	 address                       varchar(50) NOT NULL,
	 privacy                       tinyint NULL,
       zip_or_postcode               int NULL,

       PRIMARY KEY(address_id),
                                      FOREIGN KEY(city_id) REFERENCES CITY(city_id),
             FOREIGN KEY(profile_id) REFERENCES PROFILE(profile_id),      

);


CREATE TABLE [BOOKMARK] (

	bookmark_id                    int  IDENTITY(1,1) NOT NULL,
	url                            varchar (250) NOT NULL,
	rating                         int  NULL,
	privacy                        tinyint  NULL,
	created_at                     datetime  NOT NULL,
	bookmark_category_id           int  NOT NULL,
      bookmark_sub_category_id       int  NOT NULL,

      PRIMARY KEY(bookmark_id),
      FOREIGN KEY(bookmark_category_id) REFERENCES BOOKMARK_CATEGORY (bookmark_category_id),
      FOREIGN KEY(bookmark_sub_category_id) REFERENCES BOOKMARK_SUB_CATEGORY (bookmark_sub_category_id),
 
);



CREATE TABLE [BOOKMARK_CATEGORY] (

	 bookmark_category_id          int  IDENTITY(1,1) NOT NULL,
       name                          varchar (50) NOT NULL,

       PRIMARY KEY(bookmark_category_id),
       
);



CREATE TABLE [BOOKMARK_INFO] (

	 bookmark_info_id              int  IDENTITY(1,1) NOT NULL,
	 bookmark_id                   int  NOT NULL,
	 user_id                       int  NOT NULL,
	 favorite                      bit  NOT NULL,
	 clicks                        int  NULL,
             privacy                       tinyint  NULL,
             PRIMARY KEY(bookmark_info_id),
             FOREIGN KEY(bookmark_id) REFERENCES BOOKMARK (bookmark_id),
);



CREATE TABLE [BOOKMARK_SUB_CATEGORY] (

	 bookmark_sub_category_id      int  IDENTITY(1,1) NOT NULL,
	 name                          varchar (50) NOT NULL,
       bookmark_category_id          int  NOT NULL,

       PRIMARY KEY(bookmark_sub_category_id),
       FOREIGN KEY(bookmark_category_id) REFERENCES BOOKMARK_CATEGORY (bookmark_category_id),

);


CREATE TABLE [CITY] (

	 city_id                       int  IDENTITY(1,1) NOT NULL,
	 country_id                    int  NOT NULL,
       city                          varchar (50) NOT NULL,

       PRIMARY KEY(city_id),
       FOREIGN KEY(country_id) REFERENCES  COUNTRY (country_id),
);



CREATE TABLE [COMMENT] (

	 comment_id                    int  IDENTITY(1,1) NOT NULL,
	 message                       varchar (250) NOT NULL,
	 created_at                    datetime  NOT NULL,
	 status_id                     int  NOT NULL,
       friend_id                     int  NOT NULL,

       PRIMARY KEY(comment_id),
       FOREIGN KEY(friend_id) REFERENCES FRIEND (friend_id),
       FOREIGN KEY(status_id) REFERENCES STATUS (status_id),
);


CREATE TABLE [CONNECTION] (

	 connection_id                 int  IDENTITY(1,1) NOT NULL,
	 connection_user_id            int  NOT NULL,
	 user_id                       int  NOT NULL,
       created_at                    datetime  NOT NULL,

       PRIMARY KEY(connection_id),
       FOREIGN KEY(connection_user_id) REFERENCES USER (connection_user_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);



CREATE TABLE [COUNTRY] (

	 country_id                    int  IDENTITY(1,1) NOT NULL,
             country                       varchar (50) NOT NULL,
             PRIMARY KEY(country_id),
             
);


CREATE TABLE [CV] (

	 cv_id                         int  IDENTITY(1,1) NOT NULL,
	 user_id                       int  NOT NULL,
	 date_created                  datetime  NOT NULL,
             date_updated                  datetime  NULL,
             PRIMARY KEY(cv_id),
             FOREIGN KEY(user_id) REFERENCES USER (user_id),
);


CREATE TABLE [CV_SECTION] (

	 cv_section_id                 int  IDENTITY(1,1) NOT NULL,
	 cv_id                         int  NOT NULL,
	 cv_section_name               varchar (50) NOT NULL,
	 date_created                  datetime  NOT NULL,
	 date_updated                  datetime  NULL,
             cv_section_text               varchar (500) NOT NULL,
             PRIMARY KEY(cv_section_id),
             FOREIGN KEY(cv_id) REFERENCES CV (cv_id),
);


CREATE TABLE [FEED] (

	 feed_id                       int  IDENTITY(1,1) NOT NULL,
	 feed_url                      varchar (250) NOT NULL,
	 rating                        int  NULL,
	 privacy                       tinyint  NULL,
	 created_at                    datetime  NOT NULL,
             feed_category_id              int  NOT NULL,
             PRIMARY KEY(feed_id),
             FOREIGN KEY(feed_category_id) REFERENCES FEED_CATEGORY (feed_category_id),
);


CREATE TABLE [FEED_CATEGORY] (

	 feed_category_id              int  IDENTITY(1,1) NOT NULL,
       name                          varchar (50) NOT NULL,

       PRIMARY KEY(feed_category_id),
       
);


CREATE TABLE [FEED_INFO] (

	 feed_info_id                  int  IDENTITY(1,1) NOT NULL,
	 feed_id                       int  NOT NULL,
	 user_id                       int  NOT NULL,
	 clicks                        int  NULL,
             privacy                       tinyint  NULL,
             PRIMARY KEY(feed_info_id),
             FOREIGN KEY(user_id) REFERENCES USER (user_id),
             FOREIGN KEY(feed_id) REFERENCES FEED (feed_id),
);


CREATE TABLE [FRIEND] (

	 friend_id                     int  IDENTITY(1,1) NOT NULL,
	 friend_user_id                int  NOT NULL,
	 is_subscriber                 bit  NOT NULL,
	 privacy                       tinyint  NULL,
	 created_at                    datetime  NOT NULL,
	 user_id                       int  NOT NULL,
       friend_list_id                int  NOT NULL,

       PRIMARY KEY(friend_id),
       FOREIGN KEY(friend_user_id) REFERENCES USER (friend_user_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
       FOREIGN KEY(friend_list_id) REFERENCES FRIEND_LIST_NAME (friend_list_id),

);


CREATE TABLE [FRIEND_LIST_NAME] (

	 friend_list_id                int  IDENTITY(1,1) NOT NULL,
       list_name                     varchar (50) NOT NULL,

       PRIMARY KEY(friend_list_id),
    
);


CREATE TABLE [GROUPS] (

	 group_id                      int  IDENTITY(1,1) NOT NULL,
	 created_by_user_id            int  NOT NULL,
	 group_name                    varchar (150) NOT NULL,
	 group_description             varchar (250) NOT NULL,
	 group_date_started            datetime  NOT NULL,
             group_date_ended              datetime  NULL,
             PRIMARY KEY(group_id),
             FOREIGN KEY(created_by_user_id) REFERENCES USER (created_by_user_id),
);


CREATE TABLE [LANGUAGE] (

	 language_id                   tinyint  IDENTITY(1,1) NOT NULL,
	 user_id                       int  NOT NULL,
       language                      varchar (50) NOT NULL,

       PRIMARY KEY(language_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);


CREATE TABLE [MESSAGE] (

	 message_id                    int  IDENTITY(1,1) NOT NULL,
	 message                       varchar (500) NULL,
	 created_at                    datetime  NOT NULL,
	 is_read                       bit  NOT NULL,
	 is_spam                       bit  NOT NULL,
	 to_who                        int  NOT NULL,
	 is_reply                      bit  NOT NULL,
       user_id                       int  NOT NULL,

       PRIMARY KEY(message_id),
       FOREIGN KEY(to_who) REFERENCES USER (to_who),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);


CREATE TABLE [NOTIFICATION] (

	 notification_id               int  IDENTITY(1,1) NOT NULL,
	 msg                           varchar (250) NOT NULL,
	 privacy                       int  NOT NULL,
	 created_at                    datetime  NOT NULL,
       user_id                       int  NOT NULL,

       PRIMARY KEY(notification_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);


CREATE TABLE [ORGANIZATION] (

	 organization_id               int  IDENTITY(1,1) NOT NULL,
	 organization_name             nvarchar (50) NOT NULL,
       organization_description      nvarchar (250) NULL,

       PRIMARY KEY(organization_id),
       
);


CREATE TABLE [PEOPLE_BEING_FOLLOWED] (

	 user_id                       int  NOT NULL,
	 user_being_followed_id        int  NOT NULL,
	 date_started_following        datetime  NOT NULL,
       date_stop_following           datetime  NULL,

       PRIMARY KEY(user_id, user_being_followed_id, date_started_following),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
       FOREIGN KEY(user_being_followed_id) REFERENCES USER (user_being_followed_id),

);


CREATE TABLE [PRIVACY_TYPE] (

	 privacy_type_id               int  IDENTITY(1,1) NOT NULL,
       privacy_name                  varchar (50) NOT NULL,

       PRIMARY KEY(privacy_type_id),
);


CREATE TABLE [PROFILE] (

	 profile_id                    varchar (50) NOT NULL,
	 user_id                       int  NOT NULL,
	 privacy                       tinyint  NULL,
	 dob                           datetime  NULL,
	 about_me                      varchar (160) NULL,
	 relationship                  varchar (50) NULL,
	 phone                         varchar (50) NULL,
	 interests                     varchar (250) NULL,
	 education                     varchar (250) NULL,
	 hobbies                       varchar (250) NULL,
	 fav_movies                    varchar (250) NULL,
	 fav_artists                   varchar (250) NULL,
	 fav_books                     varchar (250) NULL,
	 fav_animals                   varchar (250) NULL,
       religion                      varchar (50) NULL,
 
       PRIMARY KEY(profile_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);


CREATE TABLE [PROFILE_SECTION] (
	 profile_section_id            int  IDENTITY(1,1) NOT NULL,
	 user_profile_id               int  NOT NULL,
	 profile_section_name          varchar (50) NOT NULL,
	 profile_section_text          varchar (500) NOT NULL,
	 date_created                  datetime  NOT NULL,
       date_updated                  datetime  NULL,

       PRIMARY KEY(profile_section_id),
       FOREIGN KEY(user_profile_id) REFERENCES USER_PROFILE (user_profile_id),
);


CREATE TABLE [RECOMMENDATION] (
	 user_recommending_id          int  NOT NULL,
	 user_being_recommended_id     int  NOT NULL,
       date_of_recommendation        datetime  NOT NULL,

       PRIMARY KEY(user_recommending_id, user_being_recommended_id),
       FOREIGN KEY(user_recommending_id) REFERENCES USER (user_recommending_id),
       FOREIGN KEY(user_being_recommended_id) REFERENCES USER (user_being_recommended_id),

);


CREATE TABLE [STATUS] (

	 status_id                     int  IDENTITY(1,1) NOT NULL,
	 message                       varchar (250) NULL,
	 created_at                    datetime  NOT NULL,
	 thumbs_up                     int  NULL,
	 thumbs_down                   int  NULL,
	 privacy                       tinyint  NULL,
	 is_reply                      bit  NOT NULL,
	 user_id                       int  NOT NULL,

       PRIMARY KEY(status_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);


CREATE TABLE [THUMB_UP_DOWN] (

	 thumb_up_down_id              int  IDENTITY(1,1) NOT NULL,
	 flag                          bit  NOT NULL,
	 created_at                    datetime  NOT NULL,
	 status_id                     int  NOT NULL,
       friend_id                     int  NOT NULL,

       PRIMARY KEY(thumb_up_down_id),
       FOREIGN KEY(friend_id) REFERENCES FRIEND (friend_id),
       FOREIGN KEY(status_id) REFERENCES STATUS (status_id),
);


CREATE TABLE [USER] (

	 user_id                       int  IDENTITY(1,1) NOT NULL,
	 token                         int  NOT NULL,
	 user_name                     varchar (50) NOT NULL,
	 password                      varchar (50) NOT NULL,
	 name_first                    varchar (50) NOT NULL,
	 name_middle                   varchar (50) NULL,
	 name_last                     varchar (50) NOT NULL,
	 email_address                 varchar (50) NOT NULL,
	 picture                       varchar (250) NULL,
	 active                        bit  NOT NULL,
	 online                        tinyint  NULL,
	 gender                        nchar (10) NULL,
	 current_organization_id       int  NULL,
       created_at                    datetime  NULL,

       PRIMARY KEY(user_id),
       FOREIGN KEY(current_organization_id) REFERENCES ORGANIZATION (current_organization_id),

);


CREATE TABLE [USER_GROUP] (

	 user_id                       int  NOT NULL,
	 group_id                      int  NOT NULL,
	 date_joined                   datetime  NOT NULL,
       date_left                     datetime  NULL,

       PRIMARY KEY(user_id, group_id, date_joined),	
       FOREIGN KEY(group_id) REFERENCES GROUP (group_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);



CREATE TABLE [USER_PROFILE] (

	 user_profile_id               int  IDENTITY(1,1) NOT NULL,
	 user_id                       int NOT NULL,
	 date_created                  datetime  NOT NULL,
       date_last_updated             datetime  NULL,

       PRIMARY KEY(user_profile_id),
       FOREIGN KEY(user_id) REFERENCES USER (user_id),
);


4.	Populate the database you just created again using SQL script file loaded with sample tuples. 

•	USER tablosuna veri eklendi

INSERT INTO [USER](token,user_name,password,name_first,name_middle,name_last,email_address,picture,active,online,gender,current_organization_id,
created_at)
VALUES (33333,'duygu',33333333,'Duygu',NULL,'Özen','duygu@gmail.com',NULL,1,1,'F',NULL,GETDATE())

•	PROFILE tablosuna veri eklendi
INSERT INTO PROFILE(profile_id,user_id,privacy,dob,about_me,relationship,phone,
interests,education,hobbies,fav_movies,fav_artists,fav_books,
fav_animals,religion)
VALUES('dilara1',1,1,'1993-05-29',NULL,'İlişkisi yok',
05547032905,'Software','Ege University','Reading Books','The Green Mile','Tom Hanks','Hunger Games','Horse,Dog',NULL)


•	COUNTRY tablosuna veri eklendi
INSERT INTO COUNTRY (country) VALUES ('Turkey'),
('Germany'),
('England'),
('France')


•	CITY tablosuna veri eklendi
INSERT INTO CITY (country_id,city) VALUES (1,'İstanbul'),
(1,'İzmir'),
(2,'Berlin'),
(2,'Munich'),
(3,'London'),
(4,'Paris')
	

•	ADDREESS tablosuna veri eklendi
INSERT INTO ADDRESS (city_id,profile_id,address,privacy,zip_or_postcode)
VALUES  (2,'dilara1','Kazým Dirik Mah. Bornova',2,35100),
(5,'mehmet7','63 Princes Square',6,12000),
(3,'duygu8','Goethe Str.5/3',4,80336),
(1,'tugce10','Taksim Beyoğlu',1,34000)


•	LANGUAGE tablosuna veri eklendi
INSERT INTO LANGUAGE (language,user_id) VALUES ('Turkish',1),
('Japanese',7),
('English',8),
('Turkish',10)


•	PRIVACY_TYPE tablosuna veri eklendi
INSERT INTO PRIVACY_TYPE (privacy_name) VALUES ('Public'),
('Private'),
('Only me'),
('Only friends'),
('Friends friend'),
('Family')


•	NOTIFICATION tablosuna veri eklendi
INSERT INTO NOTIFICATION (msg,privacy,created_at,user_id)
VALUES('Tuğçe Kama sizi oyun oynamaya davet etti',3,GETDATE(),1)


•	FRIEND_LIST_NAME tablosuna veri eklendi
INSERT INTO FRIEND_LIST_NAME (list_name) VALUES (‘Yakın Arkadaşlar'),
('Akraba'),
('Okul Arkadaşları'),
('İş Arkadaşları')



•	FRIEND tablosuna veri eklendi
INSERT INTO FRIEND (friend_user_id,is_subscriber,privacy,created_at,user_id,
 friend_list_id)
values (7,1,1,'2014-12-11',1,3),                                                                              (8,0,2,'2014-12-13',1,2)
	

•	STATUS tablosuna veri eklendi

INSERT INTO STATUS (message,created_at,thumbs_up,thumbs_down,privacy,is_reply,user_id) VALUES ('Bugün hava çok güzel..',GETDATE(),3,0,1,0,10),
('Alsancak yıkılıyooooo',GETDATE(),5,0,1,0,7),
('İzmir Tiyatro Festivaline herkesi bekleriz.',GETDATE(),8,0,1,0,8),
('Sokak hayvanlarını koruyalım..',GETDATE(),3,1,1,0,1)


•	COMMENT tablosuna veri eklendi
INSERT INTO COMMENT (message,created_at,status_id,friend_id) VALUES ('Bence de çok güzel..',GETDATE(),1,8),
('Bekle ben de geliyorum',GETDATE(),2,8),
('Hangi oyunlar var?',GETDATE(),3,7)


•	THUMS_UP_DOWN tablosuna veri eklendi
INSERT INTO THUMB_UP_DOWN (flag,created_at,status_id,friend_id) VALUES (1,getdate(),1,10),
(1,GETDATE(),2,7),
(0,Getdate(),4,5)




•	MESSAGE tablosuna veri eklendi
INSERT INTO MESSAGE (message,created_at,is_read,is_spam,to_who,is_reply,user_id)
 VALUES('Kaçta buluşacağız?',2014-12-15,0,0,8,0,7),
('Yarın tiyatroya gelemiyeceğim',2014-12-15,1,0,10,0,1),
('Arıyorum arıyorum ulaşamıyorum! Nerdesin??',2014-12-14,1,0,7,1,8)


•	BOOKMARK_CATEGORY tablosuna veri eklendi
INSERT INTO BOOKMARK_CATEGORY (name) VALUES('Gruplar'),('Arkadaþlar'),('Uygulamalar'),('Sayfalar')

•	BOOKMARK_SUB_CATEGORY tablosuna veri eklendi
INSERT INTO BOOKMARK_SUB_CATEGORY (name,bookmark_category_id) VALUES('Önerilen Gruplar',1),
('Arkadaşların Grupları',1),('Grupların',1),
('Aile',2),('Okul Arkadaşları',2),
('Yakın Arkadaşlar',2),('Tanıdıklar',2),
('Haber Kaynağı',3),('Etkinlikler',3),('Oyunlar',3),
('Sayfa Akışı',4),('Sayfaları Beğen',4),('Sayfa Oluştur',4)


•	BOOKMARK tablosuna veri eklendi
INSERT INTO BOOKMARK (url,rating,privacy,created_at,bookmark_category_id,
 bookmark_sub_category_)
VALUES('egebilgisayarmuhendisligi',0,1,GETDATE(),1,1),
('KocSistemçalisanlari',0,1,GETDATE(),1,2),
('DansPartileri',0,1,GETDATE(),1,3),
('YakinArkadalar',0,1,GETDATE(),2,4),
('OkulArkadaslar',0,1,GETDATE(),2,5),
('CandyCrush',0,1,GETDATE(),3,10),
('DogumGunu',0,1,GETDATE(),3,9),
('SayfalariBegen',0,1,GETDATE(),4,12)
	
•	BOOKMARK_INFO tablosuna veri eklendi
INSERT INTO BOOKMARK_INFO(bookmark_id,user_id,favorite,clicks,privacy)
VALUES   (1,1,1,1,1),
(3,1,0,1,1),
(1,7,1,1,1),
(6,7,1,1,2),
(2,8,1,1,2),
(1,8,1,1,1),
(2,10,1,1,1),
(4,10,1,1,1),
(1,10,1,3,1)
  
•	FEED_CATEGORY tablosuna veri eklendi
INSERT INTO FEED_CATEGORY (name) VALUES('Fotoğraflar'),('Videolar'),('Gruplar'),('Takip Edilenler'),('Oyunlar'),('Arkadaşlar')



•	FEED tablosuna veri eklendi
INSERT INTO FEED (feed_url,rating,privacy,created_at,feed_category_id) VALUES('hurriyet',0,1,GETDATE(),4),
('manzara.jpg',0,1,GETDATE(),1),
('newyork.jpg',0,1,GETDATE(),1),
('onedio',0,1,GETDATE(),4),							 ('Tarkan_kisgunesi.avi',0,1,GETDATE(),2),
('egebilmuh',0,1,GETDATE(),3),
('TexasHoldemPoker',0,1,GETDATE(),5)



•	FEED_INFO tablosuna veri eklendi
INSERT INTO FEED_INFO (feed_id,user_id,clicks,privacy) VALUES(1,1,2,2),
(5,1,1,1),
(3,7,3,1),
(7,7,4,1),
(4,8,2,1),
(6,8,1,2),
(2,10,2,1),
(4,10,5,1),
(1,7,10,1),
(1,10,7,1)
	
•	ORGANIZATION tablosuna veri eklendi
INSERT INTO ORGANIZATION(organization_name,organization_description) VALUES('Koç Sistem','Koç Bilgi Grubu'),
('IBTECH','Finansbank IT'),
('Garanti Teknoloji','Garanti Bankası IT'),
('Başarsoft','Navigasyon ve Haritalama'),
('Turkcell','İletişim Teknolojileri')

•	CONNETIONS tablosuna veri eklendi
INSERT INTO CONNECTION(connection_user_id,user_id,created_at) VALUES(1,10,GETDATE()),
(8,10,GETDATE()),
(7,8,GETDATE()),
(8,7,GETDATE())

•	PEOPLE_BEING_FOLLOWED tablosuna veri eklendi
INSERT INTO PEOPLE_BEING_FOLLOWED (user_id,user_being_followed_id,date_started_following,date_stop_following)
VALUES(1,13,GETDATE(),NULL),
(1,10,GETDATE(),NULL),
(7,14,GETDATE(),NULL),
(8,14,GETDATE(),NULL)

•	RECOMMENDATION tablosuna veri eklendi
INSERT INTO RECOMMENDATION (user_recommending_id,user_being_recommended_id,
 date_of_recommendation)
VALUES(1,8,GETDATE()),
(8,13,GETDATE()),
(7,10,GETDATE()),
(10,14,GETDATE())


•	CV tablosuna veri eklendi
INSERT INTO CV (user_id, date_created,date_updated)
VALUES(1,GETDATE(),NULL),
(7,GETDATE(),NULL),
(8,GETDATE(),NULL),
(10,GETDATE(),NULL)


•	CV_SECTION tablosuna veri eklendi
INSERT INTO CV_SECTION (cv_id,cv_section_name,date_created,date_updated,cv_section_text)
VALUES(1,'Deneyim',GETDATE(),NULL,'Microsoft Student Partner Temmuz 2014'),
(1,'Yetenekler',GETDATE(),NULL,'C,C++,Oracla DB'),
(3,'Deneyim',GETDATE(),NULL,'Apple, Architecture Designer Haziran 2014'),
(3,'Yetenekler',GETDATE(),NULL,'Objective C, Ruby,Pascal,C++')


•	USER_PROFILE tablosuna veri eklendi
INSERT INTO USER_PROFILE(user_id,date_created,date_last_updated) VALUES(1,GETDATE(),NULL),
(7,GETDATE(),NULL),
(8,GETDATE(),NULL),
(10,GETDATE(),NULL)


•	PROFILE_SECTION tablosuna veri eklendi
INSERT INTO PROFILE_SECTION (user_profile_id,profile_section_name,profile_section_text,date_created,date_updated)
VALUES(2,'Diller','İngilizce Konuşma:Orta,Yazma:İyi',GETDATE(),NULL),
(3,'Diller','İngilizce Konuşma:Profesyonel, Yazma:Profesyonel, Almanca:Başlangıç',GETDATE(),NULL),
(4,'Sertifikalar','Android 101 Turkcell Eğitimi',GETDATE(),NULL)



•	GROUPS tablosuna veri eklendi
INSERT INTO GROUPS (created_by_user_id,group_name,group_description,group_date_started,group_date_ended)
VALUES(13,'Microsoft Office Apps','Microsoft Office uygulamaları ile ilgili en son bilgiler',GETDATE(),NULL),
(14,'Apple i-Phone','i-Phone kullanıcılarının buluşma noktası',GETDATE(),NULL),
(7,'Ege Üniversiteli Bilgisayar Mühendisleri','Ege mezunları burada toplanıyor',GETDATE(),NULL)


•	USER_GROUPS tablosuna veri eklendi
INSERT INTO USER_GROUP(user_id,group_id,date_joined,date_left) VALUES(1,1,GETDATE(),NULL),
(1,3,GETDATE(),NULL),
(7,1,GETDATE(),NULL),
(8,2,GETDATE(),NULL),
(10,3,GETDATE(),NULL)




5.	Write down 3 triggers for 3 different tables. Triggers should be meaninful. 


•	Rating için trigger. Clickse tıklandığı zaman rating 1 artıyor

CREATE TRIGGER [Rating_Update]
ON [BOOKMARK_INFO]
AFTER INSERT
AS BEGIN
UPDATE BOOKMARK SET BOOKMARK.rating=BOOKMARK.rating+inserted.clicks FROM BOOKMARK,inserted WHERE BOOKMARK.bookmark_id=inserted.bookmark_id
END



•	Bu trigger FEED tablosundaki rating i otomatik güncelliyor.

CREATE TRIGGER [Rating_Update_Feed]
ON [FEED_INFO]
AFTER INSERT
AS BEGIN
UPDATE FEED SET FEED.rating=FEED.rating+inserted.clicks FROM FEED,inserted WHERE FEED.feed_id=inserted.feed_id
END



•	User silinirse bağlı tablolar da siliniyor
CREATE TRIGGER [User_Delete]
ON [USER]
INSTEAD OF DELETE   
AS BEGIN
DELETE FROM PROFILE WHERE PROFILE.user_id IN(SELECT user_id FROM deleted) 

DELETE FROM STATUS  WHERE STATUS.user_id IN(SELECT user_id FROM deleted) 

DELETE FROM FRIEND WHERE FRIEND.user_id IN(SELECT user_id FROM deleted) OR FRIEND.friend_user_id IN(SELECT user_id FROM deleted)

DELETE FROM LANGUAGE WHERE LANGUAGE.user_id IN(SELECT user_id FROM deleted) 

DELETE FROM MESSAGE WHERE MESSAGE.user_id IN(SELECT user_id FROM deleted) OR MESSAGE.to_who IN (SELECT user_id FROM deleted)

DELETE FROM BOOKMARK_INFO WHERE BOOKMARK_INFO.user_id IN(SELECT user_id FROM deleted) 

DELETE FROM NOTIFICATION WHERE NOTIFICATION.user_id IN(SELECT user_id FROM deleted) 

DELETE FROM FEED_INFO WHERE FEED_INFO.user_id IN(SELECT user_id FROM deleted) 

DELETE FROM CONNECTION WHERE CONNECTION.user_id IN(SELECT user_id FROM deleted) OR CONNECTION.connection_user_id IN(SELECT user_id FROM deleted)

DELETE FROM GROUPS WHERE GROUPS.created_by_user_id IN(SELECT user_id FROM deleted) --Burda kullanıcı tarafından oluşturulan grup siliniyor

DELETE FROM USER_GROUP WHERE USER_GROUP.user_id IN(SELECT user_id FROM deleted) 

DELETE FROM PEOPLE_BEING_FOLLOWED WHERE PEOPLE_BEING_FOLLOWED.user_id IN(SELECT user_id FROM deleted) 
OR PEOPLE_BEING_FOLLOWED.user_being_followed_id IN(SELECT user_id FROM deleted) --Takip ediliyorsak bile siliniyoruz.

DELETE FROM RECOMMENDATION WHERE RECOMMENDATION.user_recommending_id IN(SELECT user_id FROM deleted) 
OR RECOMMENDATION.user_being_recommended_id IN(SELECT user_id FROM deleted)

DELETE FROM CV WHERE CV.user_id IN(SELECT user_id FROM deleted)

DELETE FROM USER_PROFILE WHERE USER_PROFILE.user_id IN(SELECT user_id FROM deleted)

DELETE FROM [USER] WHERE [USER].user_id IN(SELECT user_id FROM deleted)
END



•	Comment girildiğinde Is_reply true(1) oluyor

CREATE TRIGGER [ReplyUpdate]
ON [COMMENT]
AFTER INSERT
AS BEGIN
UPDATE STATUS SET is_reply=1 FROM STATUS,inserted WHERE  STATUS.status_id=inserted.status_id
END




6.	Write down 3 check constraints and 3 assertions. Check constraints and assertions should be meaninful. 

CHECK CONSTRAINT


Gender sahası M ya da F olabilir.

ALTER TABLE [USER]
ADD CONSTRAINT chk_Gender CHECK(gender='M' OR gender='F') 



Şifre uzunluğu min 8 max 16 karakter uzunluğunda olmalıdır.

ALTER TABLE [USER]
ADD CONSTRAINT chk_Password CHECK(len(password)>=8 and len(password)<=16)



Bir kullanıcı kendisini arkadaş olarak ekleyemez.

ALTER TABLE FRIEND
ADD CONSTRAINT chk_Friend CHECK (user_id!=friend_user_id)






ASSERTION
•	Kullanıcının doğum tarihi facebook u oluşturma tarihinden daha büyük olamaz.

CREATE ASSERTION dob_Profile
CHECK (NOT EXISTS (SELECT dob,created_at FROM [USER] as U,PROFILE as P WHERE U.user_id=P.user_id 
AND  U.created_at<=P.dob))

-------------------------------------------------------------------

CREATE TRIGGER dob_check
ON [dbo].[PROFILE]
FOR INSERT
AS 
DECLARE @created DATETIME
DECLARE @dob DATETIME
SELECT @created=[USER].created_at, @dob=inserted.dob FROM [USER],inserted WHERE [USER].user_id=inserted.user_id
IF (@created<@dob)
BEGIN
print('Hatalı doğum tarihi girişi!')
rollback transaction
END


•	Cevaplanan bir mesaj varsa  okunmuş olmalıdır.


ALTER TABLE MESSAGE
ADD CONSTRAINT chk_reply CHECK((is_reply=1 AND is_read=1) OR (is_reply=0 AND is_read=1) OR (is_reply=0 AND is_read=0))




•	Grup yaratma tarihi kapatma tarihinden büyük olamaz.


CREATE ASSERTION created_Group
CHECK (NOT EXISTS (SELECT * FROM GROUPS WHERE group_date_ended<group_date_started))
-------------------------------------------------------------------
ALTER TABLE GROUPS
ADD CONSTRAINT chk_groupDate CHECK(group_date_ended<group_date_started)






7.Write down the following SQL statements

a.	Write sample INSERT, DELETE and UPDATE statements for 3 of the tables you have chosen. 

•	  USER tablosu için işlemler

UPDATE [USER] SET current_organization_id=6 WHERE user_id=8


DELETE FROM [USER] where user_id=11


INSERT INTO [USER] (token,user_name,password,name_first,name_middle,name_last,email_address,picture,active,online,gender,current_organization_id,created_at)
VALUES(99999,'keremgunduz',88888888,'Kerem',NULL,'Gündüz','kerem@gmail.com',NULL,1,1,'M',2,GETDATE())

•	  STATUS tablosu için işlemler

UPDATE STATUS SET message='Sokak hayvanlarını koruyalım. Herkes kapısının önüne su koysun.' WHERE status_id=4



INSERT INTO STATUS VALUES('Herkese iyi yıllar..',GETDATE(),5,0,1,0,1)



DELETE FROM STATUS WHERE status_id=5

•	  CV_SECTION için işlemler

UPDATE CV_SECTION SET cv_section_text='Apple, Architecture Designer Haziran 2014, Microsoft Team Lead', date_updated=GETDATE() WHERE cv_section_id=6



INSERT INTO CV_SECTION VALUES(2,'Deneyim',GETDATE(),NULL,'Ege Üniversitesi Bilgisayar Mühendisliği N.Y.G.')




DELETE FROM CV_SECTION WHERE cv_section_id=5


b.	 Write 10 SELECT statements for the database you have implemented. 

i.

•	User tablosunda ilk adının baş harfi D olan kullanıcıların listelenmesi
SELECT * 
FROM [USER]  
WHERE name_first LIKE 'D%'



•	Profil tablosunda doğum tarihi küçükten büyüğe doğru sıralanır
SELECT * 
FROM PROFILE 
ORDER BY dob DESC


•	Bookmark tablosunda max rating olan kaydı yazdırıyoruz.

SELECT * 
FROM BOOKMARK 
WHERE rating=(SELECT MAX(rating) FROM BOOKMARK)


ii.

•	Grup kuran kullanıcıların user_id,adı_soyadı ve kurduğu grubun adını listeler.

SELECT [USER].user_id,[USER].name_first,[USER].name_last,
GROUPS.group_name 
FROM [USER],GROUPS
WHERE [USER].user_id=GROUPS.created_by_user_id



•	Yakın arkadaş listesinde arkadaşa sahip olan kullanıcıların adları,soyadları, yakın arkadailarının adları ve soyadlarını listeler

SELECT T.name_first AS user_name ,T.name_last AS user_last_name,F.name_first AS close_friend_name,F.name_last AS close_friend_last_name
FROM [USER] AS T ,[USER] AS F, FRIEND as x, FRIEND as y
WHERE ((T.user_id) IN (SELECT x.user_id  WHERE  x.friend_list_id=1) AND
(F.user_id) IN (SELECT y.friend_user_id WHERE  y.friend_list_id=1) ) AND (x.friend_id=y.friend_id)





•	Kategorisi Takip Edilenler olan sayfaların url sini,rating ini ve kategorisini listeler

SELECT F.feed_url,F.rating,FC.name 
FROM FEED AS F, FEED_CATEGORY AS FC
WHERE FC.name='Takip Edilenler' AND F.feed_category_id=FC.feed_category_id



•	Herhangi bir gruba kayıt olmayan kullanıcıların bilgilerinin listelenmesi

SELECT * 
FROM [USER] 
WHERE NOT EXISTS  (SELECT * 
                   FROM USER_GROUP 
                   WHERE USER_GROUP.user_id=[USER].user_id)


iii.

•	Bir kullanıcının facebook ve linkedinde ortak olan arkadaşların adı ve soyadını listelemesi.


SELECT U.name_first,U.name_last,F.name_first,F.name_last  FROM [USER] AS U, [USER] AS F,FRIEND,CONNECTION
WHERE (U.user_id IN(SELECT FRIEND.user_id  WHERE FRIEND.friend_user_id=CONNECTION.connection_user_id AND FRIEND.user_id=CONNECTION.user_id  )
AND F.user_id IN(SELECT CONNECTION.connection_user_id  WHERE  FRIEND.friend_user_id=CONNECTION.connection_user_id AND FRIEND.user_id=CONNECTION.user_id )) AND
(U.user_id=CONNECTION.user_id)









•	İstanbulda yaşayan kullanıcıların çalıştığı yer ile kullanıcı bilgilerini yazdırır.

SELECT U.name_first,U.name_last,O.organization_name 
            FROM [USER] AS U,ORGANIZATION AS O
WHERE U.current_organization_id=O.organization_id AND U.user_id IN (SELECT PROFILE.user_id 
    FROM PROFILE,[USER] 
    WHERE PROFILE.profile_id  IN (SELECT ADDRESS.profile_id            
                                  FROM CITY,ADDRESS 
                                  WHERE CITY.city_id=ADDRESS.city_id AND CITY.city='İstanbul'))




•	Herhangi bir kullanıcının cv sectionlarını listelemek

SELECT U.name_first,U.name_last,CS.cv_section_name,CS.cv_section_text   FROM [USER] AS U,CV_SECTION AS CS,CV
WHERE U.user_id=CV.user_id AND CS.cv_id=CV.cv_id





