# questionnairebilan
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Questionnaire - Moi au lycée de Borda</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1, h2 {
            color: #333;
        }
        .form-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input[type="text"], textarea, select {
            width: 100%;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        .radio-group, .checkbox-group {
            display: flex;
            flex-direction: column;
            gap: 5px;
            margin-top: 5px;
        }
        .radio-group label, .checkbox-group label {
            font-weight: normal;
            display: inline;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Questionnaire : Moi au lycée de Borda</h1>

        <form action="https://formsubmit.co/thierry.guichemerre@orange.fr" method="POST">
            <!-- Champs cachés pour FormSubmit -->
            <input type="hidden" name="_subject" value="Nouvelle réponse au questionnaire - Moi au lycée de Borda">
            <input type="hidden" name="_next" value="https://ton-site.com/confirmation.html">
            <input type="hidden" name="_captcha" value="false">

            <div class="form-group">
                <label for="nom">NOM :</label>
                <input type="text" id="nom" name="nom" required>
            </div>

            <div class="form-group">
                <label for="prenom">Prénom :</label>
                <input type="text" id="prenom" name="prenom" required>
            </div>

            <h2>Partie 1 : Moi au lycée de Borda</h2>

            <div class="form-group">
                <label>1. Comment te sens-tu au lycée depuis la rentrée ?</label>
                <div class="radio-group">
                    <label><input type="radio" name="q1" value="Très bien" required> Très bien</label>
                    <label><input type="radio" name="q1" value="Bien"> Bien</label>
                    <label><input type="radio" name="q1" value="Moyen"> Moyen</label>
                    <label><input type="radio" name="q1" value="Pas très bien"> Pas très bien</label>
                    <label><input type="radio" name="q1" value="Mal"> Mal</label>
                </div>
            </div>

            <div class="form-group">
                <label for="q2">2. Peux-tu expliquer pourquoi ?</label>
                <textarea id="q2" name="q2" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q3">3. Qu'est-ce qui te plaît le plus au lycée ?</label>
                <textarea id="q3" name="q3" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q4">4. Qu'est-ce qui te plaît le moins ou te pose un problème ?</label>
                <textarea id="q4" name="q4" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label>5. Te considères-tu comme attentif/ve et respectueux/se en classe ?</label>
                <div class="radio-group">
                    <label><input type="radio" name="q5" value="Oui" required> Oui</label>
                    <label><input type="radio" name="q5" value="Plutôt"> Plutôt</label>
                    <label><input type="radio" name="q5" value="Parfois"> Parfois</label>
                    <label><input type="radio" name="q5" value="Non"> Non</label>
                </div>
            </div>

            <div class="form-group">
                <label>6. Comment te sens-tu dans ton groupe classe ?</label>
                <div class="radio-group">
                    <label><input type="radio" name="q6" value="Très bien intégré(e)" required> Très bien intégré(e)</label>
                    <label><input type="radio" name="q6" value="Assez bien"> Assez bien</label>
                    <label><input type="radio" name="q6" value="Moyennement"> Moyennement</label>
                    <label><input type="radio" name="q6" value="Pas très bien"> Pas très bien</label>
                </div>
            </div>

            <div class="form-group">
                <label for="q7">7. Comment sont tes relations avec les camarades ?</label>
                <textarea id="q7" name="q7" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q8">8. Et avec les professeurs ?</label>
                <textarea id="q8" name="q8" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label>9. As-tu déjà eu des sanctions ou observations de comportement ?</label>
                <div class="radio-group">
                    <label><input type="radio" name="q9" value="Oui" required> Oui</label>
                    <label><input type="radio" name="q9" value="Non"> Non</label>
                </div>
                <label for="q9_explication">Si oui, pourquoi ?</label>
                <textarea id="q9_explication" name="q9_explication" rows="2"></textarea>
            </div>

            <h2>Partie 2 : Mon attitude d'apprenant</h2>

            <div class="form-group">
                <label>1. Ton investissement en classe :</label>
                <div class="radio-group">
                    <label><input type="radio" name="q10" value="Très bon" required> Très bon</label>
                    <label><input type="radio" name="q10" value="Correct"> Correct</label>
                    <label><input type="radio" name="q10" value="Moyen"> Moyen</label>
                    <label><input type="radio" name="q10" value="Insuffisant"> Insuffisant</label>
                </div>
            </div>

            <div class="form-group">
                <label>2. Ton travail à la maison :</label>
                <div class="radio-group">
                    <label><input type="radio" name="q11" value="Très bon" required> Très bon</label>
                    <label><input type="radio" name="q11" value="Correct"> Correct</label>
                    <label><input type="radio" name="q11" value="Moyen"> Moyen</label>
                    <label><input type="radio" name="q11" value="Insuffisant"> Insuffisant</label>
                </div>
            </div>

            <div class="form-group">
                <label>3. Tes difficultés principales :</label>
                <div class="checkbox-group">
                    <label><input type="checkbox" name="q12_devoirs" value="Devoirs"> Devoirs</label>
                    <label><input type="checkbox" name="q12_concentration" value="Concentration"> Concentration</label>
                    <label><input type="checkbox" name="q12_organisation" value="Organisation"> Organisation</label>
                    <label><input type="checkbox" name="q12_participation" value="Participation"> Participation</label>
                    <label><input type="checkbox" name="q12_autre" value="Autre"> Autre : <input type="text" name="q12_autre_texte"></label>
                </div>
            </div>

            <div class="form-group">
                <label for="q13">4. Tes matières préférées et pourquoi :</label>
                <textarea id="q13" name="q13" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q14">5. Tes matières les plus difficiles et pourquoi :</label>
                <textarea id="q14" name="q14" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q15">6. Quelle fierté ou réussite veux-tu mettre en avant pour cette première période ?</label>
                <textarea id="q15" name="q15" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q16">7. Qu'aimerais-tu améliorer pour la deuxième période ?</label>
                <textarea id="q16" name="q16" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q17">8. Quels objectifs personnels te fixes-tu ? (au moins deux)</label>
                <textarea id="q17" name="q17" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q18">9. Comment comptes-tu t'y prendre pour atteindre ces objectifs ?</label>
                <textarea id="q18" name="q18" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q19">10. Y a-t-il un sujet particulier que tu aimerais aborder avec ton professeur principal ?</label>
                <textarea id="q19" name="q19" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label for="q20">11. As-tu besoin d'un soutien, d'une aide ou d'un conseil dans un domaine précis ?</label>
                <textarea id="q20" name="q20" rows="3"></textarea>
            </div>

            <div class="form-group">
                <label>12. Vœux pour l'année prochaine :</label>
                <div class="checkbox-group">
                    <label><input type="checkbox" name="q21_premiere_generale" value="première générale"> Première générale</label>
                    <label><input type="checkbox" name="q21_premiere_technologique" value="première technologique"> Première technologique</label>
                    <label><input type="checkbox" name="q21_voie_professionnelle" value="voie professionnelle"> Voie professionnelle</label>
                    <label><input type="checkbox" name="q21_autre" value="autre"> Autre</label>
                </div>
                <div class="form-group">
                    <label>Spécialités (si première générale) :</label>
                    <input type="text" name="q21_spe1" placeholder="Spé 1">
                    <input type="text" name="q21_spe2" placeholder="Spé 2">
                    <input type="text" name="q21_spe3" placeholder="Spé 3">
                </div>
            </div>

            <div class="form-group">
                <button type="submit">Envoyer</button>
            </div>
        </form>
    </div>
</body>
</html>
