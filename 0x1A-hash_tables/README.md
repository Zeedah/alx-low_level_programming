Rewrite the previous functions using these data structures:



shash_table_t *shash_table_create(unsigned long int size);

int shash_table_set(shash_table_t *ht, const char *key, const char *value);

The key/value pair should be inserted in the sorted list at the right place

Note that here we do not want to do exactly like PHP: we want to create a sorted linked list, by key (sorted on ASCII value), that we can print by traversing it. See example.

char *shash_table_get(const shash_table_t *ht, const char *key);
