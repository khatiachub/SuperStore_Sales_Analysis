📊 E-Commerce Business Analytics (SQL + Power BI)

📌 პროექტის მიმოხილვა
პროექტის მიზანი იყო ელექტრონული კომერციის (E-Commerce) ტრანზაქციული მონაცემების დამუშავება, კომპლექსური ბიზნეს-მეტრიკების გამოთვლა SQL-ში და ინტერაქციული Dashboard-ის აგება Power BI-ში სტრატეგიული გადაწყვეტილებების მისაღებად.

🛠️ ტექნოლოგიური სტეკი

SQL Server (T-SQL): CTE, Window Functions, მონაცემთა გაწმენდა, VIEW-ების შექმნა.
Power BI: მონაცემთა მოდელირება (Snowflake Schema), DAX, ინტერაქციული ვიზუალიზაცია.

⚙️ მონაცემთა ინჟინერია (ETL & Normalization)

პროექტის ფარგლებში განხორციელდა მონაცემთა სრული ETL (Extract, Transform, Load) ციკლი და არქიტექტურული ოპტიმიზაცია:
მონაცემთა გაწმენდა (Transformation): ნედლი მონაცემები გასუფთავდა დუბლიკატებისგან, გასწორდა ტექსტური ხარვეზები (Spaces & Case issues) და სტანდარტიზირდა თარიღების ფორმატები.
მონაცემთა ნორმალიზაცია: მონაცემები დაიშალა მესამე ნორმალური ფორმის (3NF) პრინციპით. fact_Orders (ფაქტების ცხრილი) გამოიყო განზომილებების საცნობარო ცხრილებისგან (Products, Sub_Category, Category, Customer, Location).
ოპტიმიზაცია VIEW-ების დახმარებით: SQL-ში შეიქმნა წინასწარ გამართული ხედები (Views), რამაც შეამცირა Power BI-ში შესატანი მონაცემების მოცულობა და აარიდა თავი მოდელში ზედმეტი ჯოინების (Joins) წერას.

🚀 რა გაკეთდა SQL-ში? (Data & Analytics)

fact_Orders და განზომილებების ცხრილების ბაზაზე შეიქმნა ოპტიმიზებული VIEW-ები შემდეგი ანალიზისთვის:
RFM სეგმენტაცია: NTILE()-ითა და CASE WHEN-ით მომხმარებლები დაიყვნენ ქცევით სტატუსებად (მაგ. Champions, At Risk, Lost).
MoM Customer Growth: LAG() ფუნქციით განისაზღვრა აქტიური კლიენტების ბაზის თვიური ზრდა/კლების ტემპი.
კუმულაციური გაყიდვები (Running Total): გაყიდვების ჯამური ზრდა დროში, დაშლილი ბაზრებისა და კატეგორიების ჭრილში.
მოძრავი საშუალო (Moving Average): 3 და 7-დღიანი პერიოდების მოძრავი საშუალო გაყიდვების რეალური ტრენდების საჩვენებლად.
პროდუქტების შიდა ანალიზი: იდენტიფიცირდა ის წამყვანი პროდუქტები, რომელთა საშუალო გაყიდვები აჭარბებს მათივე ქვეკატეგორიის შიდა საშუალო მაჩვენებელს.

📉 რა გაკეთდა Power BI-ში? (Modeling & Visuals)

მონაცემთა მოდელირება: აიგო გამართული Snowflake სტრუქტურა 1-to-Many კავშირებით, რაც უზრუნველყოფს სწრაფ და ავტომატურ ფილტრაციას.
ვიზუალიზაცია:
Line & Area Charts: მოძრავი საშუალოს და კუმულაციური გაყიდვების დინამიკისთვის.
Slicers: ფილტრები RFM სეგმენტების, რეგიონებისა და პროდუქტის იერარქიების მიხედვით.
Leaderboards: ქვეკატეგორიის საშუალოზე მაღალი გაყიდვების მქონე პროდუქტების რეიტინგი.
<img width="872" height="495" alt="1" src="https://github.com/user-attachments/assets/5f2eba5c-e940-4e2b-9597-bd65ec3f7a03" />
<img width="876" height="490" alt="2" src="https://github.com/user-attachments/assets/e31dd4cf-9cdb-495d-abc5-908036cddcab" />
<img width="876" height="490" alt="3" src="https://github.com/user-attachments/assets/c8a07021-2583-419d-a834-afeb8b3ea2a6" />
<img width="878" height="493" alt="4" src="https://github.com/user-attachments/assets/89dc9174-3560-42ba-95e8-94dd293c9cf5" />
<img width="872" height="488" alt="5" src="https://github.com/user-attachments/assets/e8a73f12-21fa-43d8-9c4b-1aa5d0769c85" />
<img width="875" height="490" alt="6" src="https://github.com/user-attachments/assets/4062b9e6-f301-444f-883d-6565c5e7f983" />
<img width="875" height="486" alt="7" src="https://github.com/user-attachments/assets/10f5f5c4-ad5e-41c6-93fa-221a9fa12e65" />
<img width="875" height="487" alt="8" src="https://github.com/user-attachments/assets/d0d4e8c2-2e5e-49d3-8f9a-5dd78d283434" />
<img width="875" height="488" alt="9" src="https://github.com/user-attachments/assets/442a25ed-127d-4240-8101-e2de9b5ded8c" />


