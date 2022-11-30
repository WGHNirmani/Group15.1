# Group15.1
Moonshine is the best e-learning platform for Preschool children.
//importing items to the page
import { StyleSheet, Text, TouchableOpacity, View,Image} from 'react-native';
import Alphabet from './assets/Alphabet.png';
import Vegitables from './assets/Vegitables.jpg';
import Animals from './assets/Animals.webp';
import Fruits from './assets/Fruits.jpg';

const englishPage=(props) =>{
  return (
    <View style={styles.container}>
      <Text style={styles.top}>English </Text>
      
      <TouchableOpacity onPress={() => props.navigation.navigate('Alphabet')} style={styles.con1}>
        <Image source={Alphabet} style={styles.img}/>
        <Text style={styles.name}>Alphabet</Text>
      </TouchableOpacity>

      <Text></Text>

      <TouchableOpacity onPress={() => props.navigation.navigate('vegitables')} style={styles.con1}>
        <Image source={Vegitables} style={styles.img}/>
        <Text style={styles.name}>Vegetables</Text>
      </TouchableOpacity>

      <Text></Text>

      <TouchableOpacity onPress={() => props.navigation.navigate('animal')} style={styles.con1}>
        <Image source={Animals} style={styles.img}/>
        <Text style={styles.name}>Animals</Text>
      </TouchableOpacity>

      <Text></Text>

      <TouchableOpacity onPress={() => props.navigation.navigate('Alphabet')} style={styles.con1}>
        <Image source={Fruits} style={styles.img}/>
        <Text style={styles.name}>Fruits</Text>
      </TouchableOpacity>

    </View>
  );
}

// styles of the components included in the page
const styles = StyleSheet.create({
  container: {
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center',
  },
  top:{
     color: 'darkblue',
     fontSize: 30,
     marginTop: 70,
     paddingBottom: 20,
  },
  con1: {
    backgroundColor: 'lightgray',
    width: 360,
    height: 134,
    borderRadius: 18,
    paddingLeft: 15,
    flexDirection: 'row',
  },
  name: {
    color: 'blue',
    fontWeight: 'bold',
    paddingVertical: 35,
    fontSize: 27,
    paddingLeft: 16,
  },
  img: {
    marginTop: 8,
    marginBottom: 10,
    width: 175,
    height: 116,
    borderRadius: 19,
    borderWidth: 2,
    borderColor: '#fff',
  },
});

export default englishPage;
