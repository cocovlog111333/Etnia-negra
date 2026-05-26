import { useState } from "react";

const preguntas = [
  {
    pregunta: "¿Cómo se llama la celebración afropanameña declarada Patrimonio Cultural Inmaterial de la Humanidad por la UNESCO?",
    opciones: ["El Congo", "La Mejorana", "El Tamborito", "El Bullerengue"],
    correcta: 0,
    explicacion: "El Congo es una manifestación cultural afropanameña de la región de Portobelo y la Costa Arriba de Colón, declarada Patrimonio por la UNESCO en 2016."
  },
  {
    pregunta: "¿En qué provincia se concentra la mayor población afrodescendiente de raíces coloniales en Panamá?",
    opciones: ["Panamá", "Colón", "Darién", "Veraguas"],
    correcta: 1,
    explicacion: "Colón, especialmente en la Costa Arriba, es el corazón de la cultura afrocolonial en Panamá, con tradiciones que datan de la época del Virreinato."
  },
  {
    pregunta: "¿Cómo se conoce a los afrodescendientes que llegaron a Panamá desde las Antillas durante la construcción del Canal?",
    opciones: ["Afroindígenas", "Afroantillanos", "Afrocriollos", "Afrocolombianos"],
    correcta: 1,
    explicacion: "Los afroantillanos llegaron principalmente desde Jamaica, Barbados y Trinidad a finales del siglo XIX y principios del XX para trabajar en el Canal de Panamá."
  },
  {
    pregunta: "¿Qué instrumento es fundamental en la música y tradición del pueblo afropanameño?",
    opciones: ["La guitarra", "La flauta", "El tambor", "El violín"],
    correcta: 2,
    explicacion: "El tambor es el instrumento central de la cultura afropanameña, presente en el tamborito, el Congo y otras expresiones culturales."
  },
  {
    pregunta: "¿Cuál es el nombre del corregimiento conocido como cuna de la cultura afropanameña colonial?",
    opciones: ["Nombre de Dios", "Portobelo", "San Miguel", "La Palma"],
    correcta: 1,
    explicacion: "Portobelo, en Colón, es considerada la cuna de la cultura afropanameña colonial. Allí se celebran el Festival del Cristo Negro y las danzas del Congo."
  },
  {
    pregunta: "¿Qué día se celebra el Día de la Etnia Negra en Panamá?",
    opciones: ["30 de mayo", "17 de agosto", "9 de junio", "1 de octubre"],
    correcta: 1,
    explicacion: "El 17 de agosto se celebra el Día de la Etnia Negra en Panamá, conmemorando la llegada de los primeros africanos esclavizados al istmo."
  },
  {
    pregunta: "¿Qué figura histórica afropanameña lideró una comunidad de esclavos cimarrones en el siglo XVI?",
    opciones: ["Victoriano Lorenzo", "Bayano", "Urracá", "Felipillo"],
    correcta: 1,
    explicacion: "Bayano fue un líder cimarrón africano que en el siglo XVI encabezó una rebelión de esclavos y fundó comunidades libres en el istmo de Panamá."
  },
  {
    pregunta: "¿Cómo se llama el baile nacional de Panamá que tiene raíces en la cultura afropanameña?",
    opciones: ["La Cumbia", "El Tamborito", "La Punta", "El Vallenato"],
    correcta: 1,
    explicacion: "El Tamborito es el baile nacional de Panamá y tiene profundas raíces en la cultura afropanameña, con el tambor como instrumento principal."
  },
  {
    pregunta: "¿En qué barrio histórico de la Ciudad de Panamá tuvo gran presencia la comunidad afroantillana?",
    opciones: ["Casco Viejo", "El Chorrillo", "Calidonia", "Bella Vista"],
    correcta: 2,
    explicacion: "Calidonia fue un barrio emblemático donde se asentó gran parte de la comunidad afroantillana en la Ciudad de Panamá, con sus iglesias, clubes y organizaciones culturales."
  },
  {
    pregunta: "¿Cuál es el nombre de la imagen religiosa venerada en Portobelo, muy ligada a la cultura afropanameña?",
    opciones: ["La Virgen del Carmen", "El Cristo Negro", "San Martín de Porres", "La Virgen de Fátima"],
    correcta: 1,
    explicacion: "El Cristo Negro de Portobelo es una imagen profundamente venerada, especialmente por la comunidad afropanameña, y su festival cada 21 de octubre atrae miles de peregrinos."
  },
  {
    pregunta: "¿De qué continente fueron traídos los africanos esclavizados que llegaron a Panamá durante la colonia?",
    opciones: ["Asia", "Europa", "África", "Oceanía"],
    correcta: 2,
    explicacion: "Los africanos esclavizados provenían de diversas regiones de África, principalmente de África Occidental y Central, y fueron traídos por los colonizadores españoles."
  },
  {
    pregunta: "¿Cómo se llamaban las comunidades libres formadas por esclavos fugitivos en la época colonial?",
    opciones: ["Reducciones", "Palenques", "Encomiendas", "Mitas"],
    correcta: 1,
    explicacion: "Los palenques eran comunidades autónomas fundadas por esclavos cimarrones que huían de sus amos. En Panamá existieron varios palenques importantes en el siglo XVI."
  },
  {
    pregunta: "¿Qué país caribeño fue la mayor fuente de trabajadores afroantillanos para la construcción del Canal de Panamá?",
    opciones: ["Cuba", "Haití", "Jamaica", "Trinidad y Tobago"],
    correcta: 2,
    explicacion: "Jamaica fue el principal país de origen de los trabajadores afroantillanos que llegaron a Panamá para construir el Canal, tanto en la época francesa como en la estadounidense."
  },
  {
    pregunta: "¿En qué año se inauguró el Canal de Panamá, cuya construcción involucró masivamente a trabajadores afroantillanos?",
    opciones: ["1903", "1914", "1920", "1930"],
    correcta: 1,
    explicacion: "El Canal de Panamá fue inaugurado en 1914. Miles de trabajadores afroantillanos contribuyeron con su trabajo y muchos con su vida a esta obra monumental."
  },
  {
    pregunta: "¿Qué tipo de música de origen africano es muy popular en las costas panameñas, especialmente en Colón?",
    opciones: ["Salsa", "Reggae", "Calypso", "Merengue"],
    correcta: 2,
    explicacion: "El calypso, de origen caribeño y con raíces africanas, es muy popular en Colón y entre las comunidades afroantillanas de Panamá."
  },
  {
    pregunta: "¿Qué término se usa para referirse a los afropanameños cuyos ancestros llegaron durante la época colonial española?",
    opciones: ["Afroantillanos", "Afrocoloniales", "Afroindígenas", "Afrocriollos"],
    correcta: 1,
    explicacion: "Los afropanameños de raíces coloniales, también llamados 'negros coloniales' o 'afrocoloniales', son descendientes de africanos esclavizados que llegaron durante el periodo español."
  },
  {
    pregunta: "¿Cuál de estos personajes fue un destacado líder político afropanameño del siglo XIX?",
    opciones: ["Manuel Amador Guerrero", "Victoriano Lorenzo", "José Domingo Espinar", "Tomás Herrera"],
    correcta: 2,
    explicacion: "José Domingo Espinar fue un destacado militar y político afropanameño del siglo XIX, llegando a ser Jefe de Estado del Istmo en 1830."
  },
  {
    pregunta: "¿Qué organización religiosa fue especialmente importante para los afroantillanos en Panamá?",
    opciones: ["La Iglesia Católica", "La Iglesia Anglicana", "La Iglesia Luterana", "La Iglesia Ortodoxa"],
    correcta: 1,
    explicacion: "La Iglesia Anglicana (Episcopal) fue fundamental para la comunidad afroantillana en Panamá, ya que muchos venían de colonias británicas con esa tradición religiosa."
  },
  {
    pregunta: "¿Cómo se llama el género musical nacido en Panamá con fuertes influencias afroantillanas?",
    opciones: ["Cumbia panameña", "Reggaeton", "El Plena", "Tamborito urbano"],
    correcta: 1,
    explicacion: "El reggaeton tiene sus raíces en Panamá, influenciado por el reggae en español de la comunidad afroantillana. Artistas como El General fueron pioneros de este género."
  },
  {
    pregunta: "¿Qué sistema discriminatorio separaba a los trabajadores en la Zona del Canal según su raza?",
    opciones: ["Sistema de castas", "Gold Roll y Silver Roll", "Apartheid canalero", "Ley de segregación"],
    correcta: 1,
    explicacion: "El sistema Gold Roll y Silver Roll segregaba a los trabajadores en el Canal: los blancos (principalmente estadounidenses) recibían mejor pago y condiciones que los afroantillanos y latinos del Silver Roll."
  },
  {
    pregunta: "¿Cuál es la danza tradicional afropanameña que representa la resistencia de los esclavos cimarrones?",
    opciones: ["El Tamborito", "El Congo", "La Cumbia", "El Bunde"],
    correcta: 1,
    explicacion: "La danza del Congo representa simbólicamente la resistencia y la libertad de los esclavos cimarrones, parodiando a los colonizadores españoles en sus movimientos y vestuario."
  },
  {
    pregunta: "¿Qué famoso músico afropanameño fue pionero del reggaeton en español?",
    opciones: ["Rubén Blades", "El General", "Blades Wilson", "Oscar Bilbao"],
    correcta: 1,
    explicacion: "El General (Edgardo Franco) fue un pionero del reggaeton en español, con raíces afroantillanas panameñas. Sus canciones de los años 90 marcaron el inicio del género a nivel internacional."
  },
  {
    pregunta: "¿Qué región de Panamá es conocida como la 'Costa Arriba' y tiene alta población afrodescendiente?",
    opciones: ["Costa del Pacífico", "Darién Norte", "Costa Arriba de Colón", "Bocas del Toro"],
    correcta: 2,
    explicacion: "La Costa Arriba de Colón es una región con fuerte presencia afrodescendiente colonial, donde se preservan tradiciones como el Congo, el tamborito y otras expresiones culturales."
  },
  {
    pregunta: "¿Qué artista visual afropanameño es reconocido por retratar la cultura negra del istmo?",
    opciones: ["Roberto Lewis", "Adriano Herrerabarría", "Manuel Chong Neto", "Guillermo Trujillo"],
    correcta: 1,
    explicacion: "Adriano Herrerabarría es un reconocido pintor afropanameño cuya obra refleja profundamente la identidad y cultura negra del istmo de Panamá."
  },
  {
    pregunta: "¿Cuál fue la primera ciudad del continente americano fundada por esclavos liberados?",
    opciones: ["Portobelo", "Nombre de Dios", "Panamá La Vieja", "Santa Cruz de Cañas"],
    correcta: 3,
    explicacion: "Santa Cruz de Cañas, en Panamá, es reconocida como la primera ciudad fundada por esclavos liberados (cimarrones) en el continente americano, en el siglo XVI."
  },
  {
    pregunta: "¿Qué lengua criolla hablan algunos afrodescendientes en la provincia de Bocas del Toro?",
    opciones: ["Papiamento", "Guari-Guari", "Creole inglés", "Saramacano"],
    correcta: 2,
    explicacion: "En Bocas del Toro se habla un creole inglés (también llamado 'Bocas Creole'), producto de la mezcla de inglés con lenguas africanas, traído por comunidades afroantillanas."
  },
  {
    pregunta: "¿Qué celebración religiosa y cultural se realiza cada 21 de octubre en Portobelo?",
    opciones: ["Festival del Tamborito", "Festival del Cristo Negro", "Día del Cimarrón", "Feria de Colón"],
    correcta: 1,
    explicacion: "El Festival del Cristo Negro de Portobelo se celebra el 21 de octubre y es una de las peregrinaciones más importantes de Panamá, con gran participación de la comunidad afropanameña."
  },
  {
    pregunta: "¿Qué escritora afropanameña es reconocida por su poesía que reivindica la identidad negra?",
    opciones: ["Rosa María Britton", "Giovanna Benedetti", "Bessy Reyna", "Melanie Taylor"],
    correcta: 3,
    explicacion: "Melanie Taylor es una poeta afropanameña cuya obra aborda la identidad afrodescendiente, el género y la cultura negra en Panamá con gran sensibilidad literaria."
  },
  {
    pregunta: "¿Cuál es el nombre del tambor más grande usado en la música afropanameña?",
    opciones: ["Caja", "Repicador", "Pujador", "Bongó"],
    correcta: 2,
    explicacion: "El pujador es el tambor más grande en la tradición afropanameña, y junto al repicador y la caja conforman el conjunto de tambores del tamborito y otras danzas tradicionales."
  },
  {
    pregunta: "¿Qué ley panameña reconoce los derechos colectivos de los afrodescendientes en el país?",
    opciones: ["Ley 16 de 2002", "Ley 11 de 2005", "Ley 9 de 2000", "Ley 22 de 2010"],
    correcta: 1,
    explicacion: "La Ley 11 de 2005 prohíbe la discriminación racial en Panamá y reconoce derechos fundamentales de las comunidades afrodescendientes, siendo un hito en la lucha por la igualdad."
  },
];

const colores = {
  fondo: "#1a0a2e",
  card: "#2d1b4e",
  acento: "#f5a623",
  correcto: "#27ae60",
  incorrecto: "#e74c3c",
  texto: "#f0e6ff",
  boton: "#6c3fc5",
};

export default function TriviaAfropanama() {
  const [idx, setIdx] = useState(0);
  const [seleccion, setSeleccion] = useState(null);
  const [puntaje, setPuntaje] = useState(0);
  const [terminado, setTerminado] = useState(false);
  const [mostrarExp, setMostrarExp] = useState(false);

  const p = preguntas[idx];

  const elegir = (i) => {
    if (seleccion !== null) return;
    setSeleccion(i);
    if (i === p.correcta) setPuntaje(s => s + 1);
    setMostrarExp(true);
  };

  const siguiente = () => {
    if (idx + 1 >= preguntas.length) setTerminado(true);
    else { setIdx(i => i + 1); setSeleccion(null); setMostrarExp(false); }
  };

  const reiniciar = () => { setIdx(0); setSeleccion(null); setPuntaje(0); setTerminado(false); setMostrarExp(false); };

  const getBtnColor = (i) => {
    if (seleccion === null) return colores.boton;
    if (i === p.correcta) return colores.correcto;
    if (i === seleccion) return colores.incorrecto;
    return "#3d2a5e";
  };

  const getMensajeFinal = () => {
    const r = puntaje / preguntas.length;
    if (r === 1) return "¡Perfecto! Eres un experto en cultura afropanameña 🏆";
    if (r >= 0.7) return "¡Muy bien! Conoces bastante sobre la etnia negra en Panamá 🌟";
    if (r >= 0.5) return "¡Bien! Puedes aprender más sobre esta rica cultura 📚";
    return "¡Sigue aprendiendo sobre la increíble herencia afropanameña! 💪";
  };

  return (
    <div style={{ minHeight: "100vh", background: colores.fondo, display: "flex", alignItems: "center", justifyContent: "center", padding: "20px", fontFamily: "Georgia, serif" }}>
      <div style={{ maxWidth: 620, width: "100%", background: colores.card, borderRadius: 20, padding: 30, boxShadow: "0 8px 32px rgba(0,0,0,0.5)", border: "2px solid #6c3fc5" }}>

        <div style={{ textAlign: "center", marginBottom: 24 }}>
          <div style={{ fontSize: 40 }}>🥁</div>
          <h1 style={{ color: colores.acento, fontSize: 22, margin: "8px 0 4px", letterSpacing: 1 }}>Etnia Negra en Panamá</h1>
          <p style={{ color: "#b39ddb", fontSize: 14, margin: 0 }}>Trivia Cultural — 30 Preguntas</p>
        </div>

        {!terminado ? (
          <>
            <div style={{ marginBottom: 20 }}>
              <div style={{ display: "flex", justifyContent: "space-between", color: "#b39ddb", fontSize: 13, marginBottom: 6 }}>
                <span>Pregunta {idx + 1} de {preguntas.length}</span>
                <span>⭐ {puntaje} pts</span>
              </div>
              <div style={{ background: "#1a0a2e", borderRadius: 10, height: 8 }}>
                <div style={{ background: colores.acento, height: 8, borderRadius: 10, width: `${((idx + 1) / preguntas.length) * 100}%`, transition: "width 0.4s" }} />
              </div>
            </div>

            <div style={{ background: "#1a0a2e", borderRadius: 14, padding: "18px 20px", marginBottom: 20 }}>
              <p style={{ color: colores.texto, fontSize: 17, lineHeight: 1.6, margin: 0 }}>{p.pregunta}</p>
            </div>

            <div style={{ display: "flex", flexDirection: "column", gap: 12, marginBottom: 20 }}>
              {p.opciones.map((op, i) => (
                <button key={i} onClick={() => elegir(i)} style={{
                  background: getBtnColor(i), color: "#fff", border: "none", borderRadius: 12,
                  padding: "14px 18px", fontSize: 15, textAlign: "left", cursor: seleccion === null ? "pointer" : "default",
                  transition: "background 0.3s", fontFamily: "Georgia, serif", display: "flex", alignItems: "center", gap: 10
                }}>
                  <span style={{ background: "rgba(255,255,255,0.15)", borderRadius: "50%", width: 28, height: 28, display: "inline-flex", alignItems: "center", justifyContent: "center", fontSize: 13, flexShrink: 0 }}>
                    {String.fromCharCode(65 + i)}
                  </span>
                  {op}
                  {seleccion !== null && i === p.correcta && " ✓"}
                  {seleccion === i && i !== p.correcta && " ✗"}
                </button>
              ))}
            </div>

            {mostrarExp && (
              <div style={{ background: seleccion === p.correcta ? "#1a3a2a" : "#3a1a1a", border: `1px solid ${seleccion === p.correcta ? colores.correcto : colores.incorrecto}`, borderRadius: 12, padding: "14px 18px", marginBottom: 20 }}>
                <p style={{ color: colores.texto, fontSize: 14, margin: 0, lineHeight: 1.6 }}>
                  <strong style={{ color: seleccion === p.correcta ? colores.correcto : colores.incorrecto }}>
                    {seleccion === p.correcta ? "✓ ¡Correcto! " : "✗ Incorrecto. "}
                  </strong>
                  {p.explicacion}
                </p>
              </div>
            )}

            {seleccion !== null && (
              <button onClick={siguiente} style={{
                background: colores.acento, color: "#1a0a2e", border: "none", borderRadius: 12,
                padding: "14px 24px", fontSize: 16, fontWeight: "bold", cursor: "pointer", width: "100%", fontFamily: "Georgia, serif"
              }}>
                {idx + 1 >= preguntas.length ? "Ver resultado final 🏁" : "Siguiente pregunta →"}
              </button>
            )}
          </>
        ) : (
          <div style={{ textAlign: "center" }}>
            <div style={{ fontSize: 64, marginBottom: 16 }}>
              {puntaje === preguntas.length ? "🏆" : puntaje >= 21 ? "🌟" : puntaje >= 15 ? "📚" : "💪"}
            </div>
            <h2 style={{ color: colores.acento, fontSize: 24, marginBottom: 8 }}>¡Trivia completada!</h2>
            <div style={{ background: "#1a0a2e", borderRadius: 16, padding: "20px", marginBottom: 20 }}>
              <p style={{ color: colores.texto, fontSize: 18, margin: "0 0 8px" }}>Tu puntaje:</p>
              <p style={{ color: colores.acento, fontSize: 48, fontWeight: "bold", margin: "0 0 8px" }}>{puntaje}/{preguntas.length}</p>
              <p style={{ color: "#b39ddb", fontSize: 14, margin: 0 }}>{Math.round((puntaje / preguntas.length) * 100)}% correcto</p>
            </div>
            <p style={{ color: colores.texto, fontSize: 16, lineHeight: 1.6, marginBottom: 24 }}>{getMensajeFinal()}</p>
            <button onClick={reiniciar} style={{
              background: colores.acento, color: "#1a0a2e", border: "none", borderRadius: 12,
              padding: "14px 32px", fontSize: 16, fontWeight: "bold", cursor: "pointer", fontFamily: "Georgia, serif"
            }}>
              🔄 Jugar de nuevo
            </button>
          </div>
        )}
      </div>
    </div>
  );
}
