مشروع
وصف الدراجة
بنهاية هذا المشروع سيكون الطالب قادرًا على:
معرفة الفرق بين نمط البرمجة كائنية التوجه Object Oriented Programming والبرمجة الإجرائية.
إنشاء Class.
إنشاء Object.
التعامل مع الخصائص Attributes و Methods الخاصة في Objectمُعين.
تطبيق المفهوم Encapsulation.
المتطلبات Requirements
الكود الموضح أدناه يمثل وصف للخصائص والسلوك الخاص بالدراجة في المصنع ذلك الوصف يتضمن:

خصائص الدراجة، مثل الوصف description، التكلفة cost، سعر البيع sale price، وحالة الدراجة condition.
إنشاء الدراجة في المصنع.
تحديث سعر الدراجة.
بيع الدراجة.
تم كتابة الكود بنمط البرمجة الإجرائية Procedure Oriented Programming قم بإعادة كتابته ولكن باتباع نمط البرمجة كائنية التوجه Object Oriented Programming.

    def update_sale_price(bike, sale_price):
        if bike['sold'] == True:
            print('Action not allowed, Bike has already been sold')
        else:
            bike['sale_price'] = sale_price
    
    
    def sell(bike):
        bike['sold'] = True
    
    
    def create_bike(description, cost, sale_price, condition):
        return {
            'description': description,
            'cost': cost,
            'sale_price': sale_price,
            'condition': condition,
            'sold': False
        }
    
    
    bike1 = create_bike('Univega Alpina, orange', cost=100, sale_price=500, condition=0.5)
    update_sale_price(bike1, 350)
    sell(bike1)
