# Billing-System

#include <stdio.h>

int main()
{
    char name[50];
    long long phone_number;
    int customer_id;

    int body_soap, body_spray, hair_cream, hair_spray;
    int sugar, tea, coffee, rice, wheat;
    int pepsi, coke, red_bull, thumbs_up;

    int total, cosmetics_total, grocery_total, beverage_total;

    printf("TRV SUPER MARKET\n");
    printf("BILLING SYSTEM\n");
    printf("---------------------\n");
    printf("Customer Details\n");

    printf("Customer Name: ");
    scanf("%49s", name);
    printf("Customer Number: ");
    scanf("%lld", &phone_number);
    printf("Customer Id: ");
    scanf("%d", &customer_id);
    printf("--------------------\n");
    
    printf("COSMETICS\n\n");
    
    printf("Body soap (RS 10): ");
    scanf("%d", &body_soap);
    printf("Hair Cream (RS 25): ");
    scanf("%d", &hair_cream);
    printf("Body Spray (RS 35): ");
    scanf("%d", &body_spray);
    printf("Hair Spray (RS 45): ");
    scanf("%d", &hair_spray);

    printf("---------------------\n");

    printf("GROCERIES\n\n");

    printf("Sugar (RS 50): ");
    scanf("%d", &sugar);
    printf("TEA (RS 10): ");
    scanf("%d", &tea);
    printf("Coffee (RS 12): ");
    scanf("%d", &coffee);
    printf("Rice (RS 100): ");
    scanf("%d", &rice);
    printf("Wheat (RS 200): ");
    scanf("%d", &wheat);

    printf("---------------------\n");

    printf("COOL DRINKS\n\n");

    printf("Pepsi (RS 40): ");
    scanf("%d", &pepsi);
    printf("Coke (RS 40): ");
    scanf("%d", &coke);
    printf("RED BULL (RS 100): ");
    scanf("%d", &red_bull);
    printf("Thumbs UP (RS 100): ");
    scanf("%d", &thumbs_up);

    printf("---------------------\n");
   
    int boso = 10 * body_soap;
    int hc = 25 * hair_cream;
    int hs = 45 * hair_spray;
    int bosp = 35 * body_spray;
    cosmetics_total = boso + hc + hs + bosp;

    printf("Body Soap: %d RS\n", boso);
    printf("Hair Cream: %d RS\n", hc);
    printf("Hair Spray: %d RS\n", hs);
    printf("Body Spray: %d RS\n", bosp);
    printf("Total Cosmetics Price: %d RS\n", cosmetics_total);

    printf("---------------------\n");

    int s = 50 * sugar;
    int t = 10 * tea;
    int c = 12 * coffee;
    int r = 100 * rice;
    int w = 200 * wheat;
    grocery_total = s + t + c + r + w;

    printf("Sugar: %d RS\n", s);
    printf("TEA: %d RS\n", t);
    printf("Coffee: %d RS\n", c);
    printf("Rice: %d RS\n", r);
    printf("Wheat: %d RS\n", w);
    printf("Total Grocery Price: %d RS\n", grocery_total);

    printf("---------------------\n");

    int pep = 40 * pepsi;
    int cok = 40 * coke;
    int rebl = 100 * red_bull;
    int thmup = 100 * thumbs_up;
    beverage_total = pep + cok + rebl + thmup;
    
    printf("Pepsi: %d RS\n", pep);
    printf("Coke: %d RS\n", cok);
    printf("RED BULL: %d RS\n", rebl);
    printf("Thumbs UP: %d RS\n", thmup);
    printf("Total Cool drinks: %d RS\n", beverage_total);

    printf("---------------------\n");

    total = cosmetics_total + grocery_total + beverage_total;

    printf("Total Amount: %d RS\n", total);

    printf("---------------------\n");
   
    printf("------------------------------------------------\n");

    printf("TVR SUPER MARKET \n\n");

    printf("Customer Name: %s\n", name);
    printf("Customer Phone Number: %lld\n", phone_number);
    printf("Customer Id: %d\n", customer_id);

    printf("Product Name                 Quantity                       Price\n\n");
    printf("Body soap                       %d                         %d\n", body_soap, boso);
    printf("Hair Cream                      %d                         %d\n", hair_cream, hc);
    printf("Hair Spray                      %d                         %d\n", hair_spray, hs);
    printf("Body Spray                      %d                         %d\n", body_spray, bosp);

    printf("Sugar                           %d                         %d\n", sugar, s);
    printf("TEA                             %d                         %d\n", tea, t);
    printf("Coffee                          %d                         %d\n", coffee, c);
    printf("Rice                            %d                         %d\n", rice, r);
    printf("Wheat                           %d                         %d\n", wheat, w);

    printf("Pepsi                           %d                         %d\n", pepsi, pep);
    printf("Coke                            %d                         %d\n", coke, cok);
    printf("RED BULL                        %d                         %d\n", red_bull, rebl);
    printf("Thumbs UP                       %d                         %d\n", thumbs_up, thmup);

    printf("Cosmetic Total Price : %d\n\n", cosmetics_total);
    printf("Grocery Total Price : %d\n\n", grocery_total);
    printf("Cool Drinks Price : %d\n\n", beverage_total);
    printf("Total price : %d\n\n", total);
    printf("------------------------------------------------\n");

    return 0;
}
