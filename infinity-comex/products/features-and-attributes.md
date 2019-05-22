# Features and attributes

**Why add features to the catalog?**

Our recommendations engine creates a statistical model that tells you what items are likely to be liked or purchased by a customer. When you have a new product that has never been interacted with it is not possible to create a model on co-occurrences alone. Let's say you start offering a new "Intel processor" in your store, since you have never sold that processor before you cannot tell what other items to recommend with that processor.

That said, our engine knows information about that processor \(i.e. brand, , etc.\), then the engine can learn from other products with similar features. For instance, you have sold violin's in the past and usually people that buy violins tend to buy classical music CDs and sheet music stands. The system can find these connections between the features and provide recommendations based on the features while your new violin has little usage.

Features and attributes are created as part of the product creation process. The SAR algorithm that is used to train the model will automatically detect the strength of each of the features based on the transaction data.

**Features are Categorical**

You should create features that resemble a category. For instance, price: 9.34 is not a categorical feature. On the other hand, a feature like "Price Range: Under 10 Dollars" is a categorical feature. Another common mistake is to use the name of the item as a feature. This would cause the name of an item to be unique so it would not describe a category. Make sure the features represent categories of items.

**How many/which features should I use?**

You should use less than 20 features.

**When are features actually used?**

Features are used by the model when there is not enough transaction data to provide recommendations on transaction information alone. So features will have the greatest impact on “cold items” – items with few transactions. If all your items have sufficient transaction information you may not need to enrich your model with features.

#### 

