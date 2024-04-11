model Product {
  // existing fields...

  quantity  Int      @default(0)
  sold      Int      @default(0)
  sku       String?  // Stock Keeping Unit, optional
  weight    Float?   // Weight of the product, optional
  dimensions String? // Dimensions of the product, optional
  materials String?  // Materials used in the product, optional
  rating    Float?   // Average rating, optional

  // existing fields...
}


model Order {
  // existing fields...

  paymentMethod String? // Method of payment, optional
  shippingCost  Float?  // Cost of shipping, optional
  taxAmount     Float?  // Tax amount, optional
  discount      Float?  // Discount on the order, optional
  totalAmount   Float?  // Total amount after adding tax and shipping cost and subtracting discount, optional
  trackingNumber String? // Tracking number for the order, optional
  deliveryDate  DateTime? // Expected delivery date, optional

  // existing fields...
}