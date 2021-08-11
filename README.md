"# Django_full_Ecom_App" 

 Easy CSE Learn
Easy CSE Learn
1 month ago
Sorry to mistake  .Change line number 37 & 43  in views.py of order app , use get rather than filter . 
Change it 
data = ShopCart.objects.filter(
                    product_id=id, user_id=current_user.id)
to 

data = ShopCart.objects.get(
                    product_id=id, user_id=current_user.id)
