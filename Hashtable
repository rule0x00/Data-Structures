# Creating a Hash Table in Python

class HashTable:
    def __init__(self):
        self.MAX = 10
        self.arr = [None for i in range(self.MAX)]
        
    def get_hash(self, key):
        #this will return the index using ASCII sum calc method
        h = 0
        for char in key:
            ascii_value = ord(char)
            h+=ascii_value
        index = h%10
        return index
    
    def add_to_hashtable(self, key, val):
        index = self.get_hash(key)
        self.arr[index] = val;
        return self.arr
    
    def get_value(self, key):
        return self.arr[key]
    
    #for better readability
    def __setitem__(self, key, val):
        index = self.get_hash(key)
        self.arr[index] = val;
        print(self.arr)
    
    def __getitem__(self, key):
        print(self.arr[self.get_hash(key)])
    
if __name__ == "__main__":
    hashtable = HashTable()
    #print(hashtable.get_hash('efgh'))
    #print(hashtable.add_to_hashtable("abcd", "efgh"))
    hashtable["abcd"] = 24
    hashtable["abcd"]
        
