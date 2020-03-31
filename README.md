# Practicing clean code writing C#
- Code Smells
```
Mysterious Names                Improved Naming

SqlDataReader dr1;              SqlDataReader dataReader;  or  SqlDataReader reader;
int od;                         int overdueDays;
void Button_Click();            void CheckAvailabitity_Click();
class Page1{}                   class ViewCustomerPage;


Meaningless Names

void BeginCheckFunctionality_StoreClientSideCheckboxIDsArray();
```
___
```
Names with Encodings                

int iMaxRequests;                   
var m_objCollection = new StringCollection();


Improved Naming

int maxRequests;
var countryNames = new StringCollection();
```
___
```
Ambiguous Names - what does this code do?

bool MultiSelect() {}
incidentNameId;


Noisy Name

Customer theCustomer;
List<Customer> listOfApprovedCustomers;

Improved Naming

Customer customer;
List<Customer> approvedCustomers;
```
___

- Inconsistent Naming Conventions
```
Customer GetCustomer(int _id);
Customer saveCustomer(Customer GetCustomer);
private int customerId;
```
- .Net Naming Conventions: PascalCase and camelCase
```
public class Customer
{
  private int _id;
  public string Name { get; set; }
  public void Charge(int amount)
  {
    var tax = 0;
  }
}
```
