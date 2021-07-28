```CPP
/**
 * Fonction qui cherche si un objet de type T est présent dans une liste contenant des objets T
 * Renvoie vrai si l'objet est trouvé, faux sinon
 * Les objets doivent avoir une fonction getId().
 */
template<typename T>
bool isObjectInList(const T& obj, std::list<T> list) {
	bool found = false;
    auto exists = std::find_if(list.begin(), list.end(),
                               [&] (const T& t) {return t.getId() == obj.getId(); });
    if (exists != list.end()) {
        found = true;
    }
    return found;
}

/**
 * Fonction cherche si un objet T avec l'ID spécifié est dans une liste contenant des objets T
 * Renvoie vrai si l'objet est trouvé, faux sinon
 * Les objets doivent avoir une fonction getId().
 */
template<typename T>
bool isIdInList(const int id, std::list<T> list) {
    bool found = false;
    auto exists = std::find_if(list.begin(), list.end(),
                               [&] (const T& t) {return t.getId() == id; });
    if (exists != list.end()) {
        found = true;
    }
    return found;
}

/**
 * Fonction qui supprime un objet d'une liste d'objets T si son ID correspond à l'ID spécifié.
 * Renvoie vrai si l'objet a été trouvé et supprimé, faux sinon
 * Les objets doivent avoir une fonction getId().
 */
template<typename T>
bool rmInListIfIdFound(int id_to_rm, std::list<T> list) {
    bool removed = false;
    list.remove_if([&] (const T& t) {
        bool found = t.getId() == id_to_rm;
        if(found){
            removed = true;
        }
        return found;
    });
    return removed;
};
```
