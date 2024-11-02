# showing-the-code-snippet-for-the-UPDATE-test-case-1-pt-
def test_list_all_products(self):
    response = self.client.get("/products")
    assert response.status_code == 200

def test_find_product_by_category(self):
    response = self.client.get("/products?category=electronics")
    assert response.status_code == 200
