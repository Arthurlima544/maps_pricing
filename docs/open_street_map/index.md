## **Open Street Map**

### **Descrição**

Um projeto colaborativo e gratuito que cria e fornece dados geográficos de todo o mundo, incluindo mapas, navegação, planejamento e análise. 

### **Features**

Conta com uma serie de funcionalidades:

- Posicao atual
- Criar Marcador
- Zoom
- Calcular Distâncias
- Clicar em marcador
- Definir Tiles°

° Tiles são pequenos blocos ou pedaços do mapa (geralmente em formato de imagem) que são carregados e montados no cliente (navegador ou aplicativo) para formar um mapa completo.

### **Custos**

Free

### **Documentação**

Por ser opensource a documentacao não é das melhores.

### **Integração com flutter**

Conta com um plugin para auxiliar a integração com o flutter, que pode ser acessado pelo [**Link**](https://pub.dev/packages/flutter_osm_plugin).


Para habilitar no projeto precisamos habilitar o **multidex**.

Exemplo Simples mostrando o mapa:

``` dart
import 'package:flutter/material.dart';
import 'package:flutter_osm_plugin/flutter_osm_plugin.dart';

void main() async {
  WidgetsFlutterBinding.ensureInitialized();
  runApp(const MyApp());
}

class MyApp extends StatefulWidget {
  const MyApp({super.key});

  @override
  State<MyApp> createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  MapController controller = MapController(
    initPosition: GeoPoint(latitude: -15.792881, longitude: -47.901361),
  );

  @override
  void dispose() {
    controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      theme: ThemeData.light(useMaterial3: true),
      initialRoute: "/home",
      routes: {
        "/home": (context) => Scaffold(
              appBar: AppBar(
                title: const Text('home'),
              ),
              body: OSMFlutter(
                controller: controller,
                osmOption: OSMOption(
                  userTrackingOption: const UserTrackingOption(
                    enableTracking: true,
                    unFollowUser: false,
                  ),
                  zoomOption: const ZoomOption(
                    initZoom: 18,
                    minZoomLevel: 3,
                    maxZoomLevel: 19,
                    stepZoom: 1.0,
                  ),
                  userLocationMarker: UserLocationMaker(
                    personMarker: const MarkerIcon(
                      icon: Icon(
                        Icons.location_history_rounded,
                        color: Colors.red,
                        size: 48,
                      ),
                    ),
                    directionArrowMarker: const MarkerIcon(
                      icon: Icon(
                        Icons.double_arrow,
                        size: 48,
                      ),
                    ),
                  ),
                  roadConfiguration: const RoadOption(
                    roadColor: Colors.yellowAccent,
                  ),
                  markerOption: MarkerOption(
                    defaultMarker: const MarkerIcon(
                      icon: Icon(
                        Icons.person_pin_circle,
                        color: Colors.blue,
                        size: 56,
                      ),
                    ),
                  ),
                ),
              ),
            ),
      },
    );
  }
}
```

### **Feedbacks**

O Mapbox (uma das soluções apresentadas) utilizam os dados do OSM para fornecer serviços de navegação e mapas offline

## **links**

- [Open Street Map - About](https://www.openstreetmap.org/about)
- [OSM plugin](https://pub.dev/packages/flutter_osm_plugin)