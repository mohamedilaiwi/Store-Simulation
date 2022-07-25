import java.util.*;

public class ShoppingCart {
   private HashMap<String, Item> cart;  
   
   public ShoppingCart() {
      cart = new HashMap<>();
   }
   
   public void add(String product, int price) {
      if (cart.keySet().contains(product)) {
         increaseQuantity(product);
      }
      else {
      cart.put(product, new Item(product, price));
      }
   }
   
   public int price() {
      int price = 0;
      for(Item m : cart.values())
      {
         price += m.price();
      }
      
      return price;
   }
   
   public void increaseQuantity(String product) {
      this.cart.get(product).increaseQuantity();
   }
   
   public void print() {
      for (String m : cart.keySet()){
         System.out.println(cart.get(m).toString());
      }
   }
}
