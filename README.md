class RevenueSystem:
    def _init_(self):
        self.revenue_list = []

    def collect_revenue(self, amount, source):
        """Collect revenue from a specified source."""
        if amount <= 0:
            raise ValueError("Revenue amount must be positive.")
        revenue = {
            'amount': amount,
            'source': source
        }
        return revenue
def add_revenue(self, amount, source):
        """Add collected revenue to the tracking list."""
        revenue = self.collect_revenue(amount, source)
        self.revenue_list.append(revenue)
        print(f"Revenue collected: {amount} from {source}")

    def total_revenue(self):
        """Calculate the total revenue collected."""
  total = sum(item['amount'] for item in self.revenue_list)
        return total

    def summary(self):
        """Print the summary of all collected revenues."""
        print("Revenue Summary:")
        for revenue in self.revenue_list:
            print(f"Source: {revenue['source']}, Amount: {revenue['amount']}")
        print(f"Total Revenue: {self.total_revenue()}")
def main():
    system = RevenueSystem()
    system.add_revenue(1000, "Client A")
    system.add_revenue(500, "Client B")
    system.add_revenue(1500, "Client C")
    
    system.summary()

if _name_ == "_main_":
    main()
