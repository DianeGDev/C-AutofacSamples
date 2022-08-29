using System;

namespace AutofacDemos
{
  public class Loan
  {
    public string Currency { get; set; }
    public int Amount { get; set; }

    public Loan(string currency, int amount)
    {
      if (currency == null)
      {
        throw new ArgumentNullException(paramName: nameof(currency));
      }
      Currency = currency;
      Amount = amount;
    }


  }

  public class DelegateFactories
  {
    // Func<T>
  }
}