 ამ დავალებაში თქვენ მოგიწევთ შექმნათ კლასი Racer. ქვემოთ აღწერილია თუ რა ახასიათებს racer-ს. 
 ამას გარდა საჭიროა driver, რომელშიც შექმნით racer ტიპის ობიექტებს რათა დატესტოთ კლასის ფუნქციები.

თქვენი Racer კლასი უნდა შეცავდეს შემდეგს:
კლასის ცვლადები:
●	A string  - ცხენის სახელი
●	A string - ჟოკეის სახელი
●	A double - ცხენის წონა 
●	A double - ჟოკეის წონა
●	An int - ჟოკეის ასაკი
●	A char - ცხენის სქესი
●	A bool for defeat (თუ ცხენი წააკებს დოღს)
●	A bool for injured (თუ ცხენი დაშავდება დოღის დროს )
●	A bool for allowed (თუ ცხენს ექნება უფლება მიიღოს მონაწილეობა შეჯიბრში)

კლასის ფუნქციები:
●	Default constructor - რომელიც შექმნის racer-ს, defeat და injured თავდაპირველად იქნება false, ხოლო allowed true
●	Explicit value constructor - რომელსაც გადასცემთ ცხენის და ჟოკეის სახელებს, მათ წონას, ცხენის ასაკსა და სქესს. 
defeat და injured თავდაპირველად იქნება false, ხოლო allowed true
●	ბეჭდვის ფუნქცია რომელიც გამოიტანს racer-ის ატრიბუტებს.
●	Age_me ფუნქცია რომელიც არაფერს აბრუნებს მაგრამ ზრდის ობიექტის ასაკს (ცხენის). თუ მრბოლელი ცხენის ასაკი 6 წელზე ნაკლებია, 
მაშინ შანსი იმისა რომ ის დოღის დროს დაშავდება არის 25%, თუ ასაკი 6დან 13წლამდეა მაშინ დაშავების შანსები 3%-მდე მცირდება. გარდა ამისა, 
შანსი იმისა რომ 13 წელს გადაცილებულ ცხენებს შეჯიბრებაზე არ დაუშვებენ 80%-ია, ასევე უნდა გაითვალისწინოთ რომ დაშავებული ცხენებიც არ დაიშვებიან დოღზე.
●	Race ფუნქცია რომელიც სხვა racer ობიექტს იღებს პარამეტრად, ფუნქცია განკუთვნილია ორ ცხენს შორის გამარჯვებულის გამოსავლენად, 
გამარჯვებულის დადგენა კი შესაძლებელია ცვლადით “fight_ratio” რომელიც გამოითვლება შემდეგნაირად:
((პირველი ცხენის წონას + მეორე ცხენის წონა) / (პირველი ჟოკეის წონას + მეორე ჟოკეის წონა)) * 50, თქვენ უნდა აირჩოთ რენდომ რიცხვი 1დან 100მდე, 
თუ რენდომ რიცხვი პატარა იქნება fight_ratio ზე მაშინ ტურნირის გამარჯვებული პირველი ცხენი იქნება, თუ მეტი მაშინ მეორე ცხენი. 

შენიშვნა: კარგად დაფიქრდით ზემოთაღნიშნული ფუნქციების დაწერასა და გამოყენებაზე. არსებობს გარემოებები, 
როდესაც ზოგიერთი ფუნქციის გამოყეება შეიძლება არც დაგჭირდეთ. მაგ: თუ ცხენი დაშავებულია Racer ფუნქციის გამოყენება საჭირო აღარ იქნება.

დავალების ატვირთვამდე თქვენმა პროგრამამ სრულიად უნდა დატესტოს Racer კლასი, უნდა გამოიძახოთ ყველა ფუნქცია Racer კლასიდა, 
უნდა დაბეჭდოთ ობიექტის მონაცემები ფუნქციის დაძახებამდე და დაძახების შემდეგ. 

როგორც ყველა წინა დავალება, თქვენ შეფასდებით მუდმივების სათანადო გამოყენების საფუძველზე. გარდა ამისა, ფუნქციების პარამეტრები, 
რომლებიც არ შეიცვლება ფუნქციაში, უნდა იყოს მუდმივი. Racer კლასს აუცილებლად უნდა ჰქონდეს შესაბამისი მუტატორები და აქსესორები.

შენიშვნა: rand() ფუნქციის გამოყენებამდე გთხოვთ გამოიყენოთ srand((unsigned int)time(0)); სხვადასხვა შემთხვევითი რიცხვების შესაქმნელად.
