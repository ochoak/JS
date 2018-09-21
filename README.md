# La verdad que me habria gustado meterle un poco más de lógica, pero lo he estado haciendo sacando ratos. 
# Pero vamos, lo importante es queria que lo tuviérais cuanto antes, se que estáis justos de tiempo con el procesos de selección. 
# 
# Hago pocas validaciones, la principal es que el objeto exista. Luego una vez que verifico si existe, comprueba que el obj tenga las propiedades que vamos a meter a cada input:
# 
# - en el caso del type, si no viene por defecto lo hago tipo "text"
# - en el caso del name, si existe le pongo name.
# - en el caso del id, si existe se lo pongo en caso contrario creo uno random. Aqui se puede comprobar que no esté repetido y en caso de que no exista para varios input se puede definir el random al principio y luego secuencialmente ir asigándolos.
# 
#   idrandom= random();
#   <input id="input'+ idrandom">
#   idrandom = idrandom + 1;
#   <input id="input'+ idrandom">
#   idrandom = idrandom + 1;
#   etc...
# 
# - en el caso de required, primero comprueba que este y si es así, en caso de TRUE, lo añado.
# 
# He definido diferentes objetos para ver distintos comportamientos: uno vacio, uno con submit o solo inputs de texto.
# 
# Al objeto se puede añadir un campo label y  añadirlo al input: 
#   label: "label del campo" // string
# 
#   <label for="nameInput"> Texto </label>
#   <input type="loquesea" name="nameInput" id="">
# 
# Las funciones se pueden encapsular más, para hacerlas más funcionales.
