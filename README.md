# MarianaSernaGETAclubAssignment
A repository with the technical art assignment for GETA Club

Dentro de este Readme se pueden encontrar los siguientes puntos de la prueba técnica resueltos:

URP:

1. X
2. Los 3 efectos de postprocesamiento que se pueden evidenciar son Tone Mapping, Bloom, Vignette y Color Adjustments, la idea del uso de estos como se encuentran son para alterar
principalmente las saturaciones de los colores y el Bloom para dar unos brillos más notorios y estéticos.
3. X

Shaders:

1. Las texturas usadas para este shader fueron del siguiente paquete:
 - https://assetstore.unity.com/packages/3d/environments/fantasy/polyart-ancient-village-pack-166022

Se realizó la construcción del shader para un terreno con las siguientes características:

Nombre del material: Terrain_Mat
Nombre del material: Terrain_Shader

 - BaseMap. (Mapa difuso.)
 - NormalMap.
 - RoughnessMap. 
 - NormalStrength. (Un slider que va de 0 a 10 para permitir que se marquen las normales a gusto, aún manteniendo un márgen.)
 - Roughness. (Un slider que va de 0 a 1 que permite escoger el valor con el que se va a marcar qué tan liso o no es el material.)

2. Para realizar el shader para simular pintura de carro realista se usó el siguiente package:
- https://assetstore.unity.com/packages/3d/vehicles/land/realistic-car-7-v5-206447

Nombre del material: CarPaint_Mat
Nombre del material: CarPaint_Shader

Tiene las siguientes características expuestas:

 - BaseMap. (Mapa difuso.)
 - Color. (Para darle un tinte de color al mapa difuso.)
 - Smoothness. (Un slider que va de 0 a 1 para mostrar qué tan liso o rugoso es el material, esto es usago principalmente para lograr que un material sea especular.)
 - Metallic. (Un slider que va de 0 a 1 para indicar qué tan metálico es el elemento.)
 - NoiseScale. (Un flotante que va a indicar qué tan grande o pequeño será un SimpleNoise.)
 - NoiseOpacity. (Al hacer uso de un SimpleNoise en el Shader Graph para simular las pinturas de los carros que generalmente tienen unos pequeños brillos, a este se le agregó un slider de
 0 a 1 para marcar la opacidad de este mismo por medio de un Blend en modo Overlay.)
 - CubeMap. (Para que la pintura tenga la reflexión del entorno en que se encuentra.)

Partículas:

1. Para visualizar la ejecución del VFX, presionar la tecla "F."

Para este ejercicio se hizo uso de un asset y material de piedra del siguiente paquete:
 - https://assetstore.unity.com/packages/3d/environments/fantasy/polyart-ancient-village-pack-166022

Se realizó una variedad de sprites para crear un efecto visual con la temática de: El poder de la madre naturaleza.

Sprites:
 - Clouds.
 - Floor.
 - Leaf.
 - NatureCircle.
 - Smoke.
 - Trail.
 - VineSprite.

Se descargó el modelo de xBot y una animación de Idle y Ataque en Mixamo:
https://www.mixamo.com/#/

Se realizó la construcción de un script simple para el showcase del efecto visual acompañado de la animación, en este se integra el componente del animator para que se instancie al darle
como input "F" una animación junto al VFX por medio de un trigger.

Se hizo la creación de un modelo en Blender (Vines_Model) por medio de curvas de Bezier para simular unas enredaderas que van a crecer por medio de un shader (VineGrowing_VFX_Shader) con
el Alpha Clipping teniendo en cuenta las UVs del modelo y a través de los Custom Vertex Streams para realizar el manejo de este a través del Particle System de Unity.

También se hizo una pequeña recreación de este mismo efecto por medio de un sprite (VineSprite) para realizar una pequeña anticipación al efecto secundario o el Release de la animación,
el principio del shader (VineSprite_VFX_Shader) es parecido al de 3D solo que su funcionamiento es por medio de la transparencia y el alpha directamente de los blancos y negros, y sus UVs,
haciendo un manejo de los elementos por medio del Custom Data también.

Como tal las diferentes partículas se fueron recreando según el efecto y comportamiento deseado para cada uno de los elementos que lo componen.

Código:

1. X

Se dejó habilitado en todo caso el camera controller con el que venía el proyecto por Default para facilidad de navegación en la escena.
Inputs de la cámara:

 - Q.
 - W.
 - E.
 - A.
 - S.
 - D.

Git:

1. Link al repositorio: https://github.com/MariSerna371/MarianaSernaGETAclubAssignment
2. Este es el Readme con la descripción de lo realizado.
3. El repositorio cuenta con más de 3 commits en él.