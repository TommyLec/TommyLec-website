<script>
	import Contact from '$lib/components/contact.svelte';
	import Experience from '$lib/components/experience.svelte';
	import Hero from '$lib/components/hero.svelte';
	import Project from '$lib/components/project.svelte';
	import Skill from '$lib/components/skill.svelte';
</script>

<Hero />

<section id="skills" class="container mx-auto">
	<h1 class="my-5 text-center text-3xl font-bold text-[#009688]">Compétences</h1>
	<div class="mx-auto grid w-fit grid-cols-4 gap-5">
		<Skill title="Svelte" icon="ri:svelte-fill" highlight />
		<Skill title="Java" icon="devicon-plain:java" highlight />
		<Skill title="Docker" icon="mdi:docker" highlight />
		<Skill title="Angular" icon="devicon-plain:angular" highlight />
		<Skill title="Spring boot" icon="simple-icons:springboot" />
		<Skill title="ReactJS" icon="ri:reactjs-fill" />
		<Skill title="JavaScript" icon="mdi:language-javascript" />
		<Skill title="TypeScript" icon="mdi:language-typescript" />
		<Skill title="Tailwind" icon="mdi:tailwind" />
		<Skill title="HTML" icon="mdi:language-html5" />
		<Skill title="CSS" icon="mdi:language-css3" />
		<Skill title="Git" icon="mdi:git" />
		<Skill title="PostgreSQL" icon="devicon-plain:postgresql" />
	</div>
</section>

<section id="experiences" class="container mx-auto mt-30">
	<h1 class="my-5 text-center text-3xl font-bold text-[#009688]">Expériences</h1>
	<div class="grid gap-10">
		<Experience title="Freelance" poste="Ingénieur Logiciel">
			Conception et développement d’un boilerplate SaaS clé en main, conçu pour les développeurs
			souhaitant lancer rapidement des applications web self hosted avec des outils modernes et
			open-source.

			<ul class="mt-5 list-inside list-disc">
				<li>
					Optimisation des coût : infrastructure cloud et services tiers réduits au strict minimum,
					évitant les abonnements à des services tiers coûtants.
				</li>
				<li>
					Performances accrues : temps de réponse des API réduit de 30% grâce à des optimisations
					backend et caching intelligent.
				</li>
			</ul>

			{#snippet more()}
				Fonctionnalités :

				<ul class="mt-5 list-inside list-disc">
					<li>
						Authentification avancée : Email/Password, 2FA, Google OAuth, Passkeys, protection
						anti-spam, validation de mot de passe robuste.
					</li>
					<li>
						Gestion des paiements intégrée : Implémentation de Paddle pour la gestion des
						abonnements et paiements uniques.
					</li>
					<li>
						Infrastructure email scalable : Support de Plunk et AWS SES pour l’envoi transactionnel
						et marketing.
					</li>
					<li>Déploiement automatisé : Scripts CI/CD optimisés, orchestration via Coolify API.</li>
				</ul>
			{/snippet}
		</Experience>
		<Experience title="Capgemini" poste="Ingénieur Logiciel">
			Mission de maintenance et d'évolution d’une application interne critique, dans un cadre de
			développement Agile (Scrum/Kanban), en garantissant stabilité, performance et évolutivité.

			<ul class="mt-5 list-inside list-disc">
				<li>
					Réduction du temps de chargement de l'application de 30% grâce à des optimisations SQL et
					backend.
				</li>
				<li>
					Stabilisation de la plateforme avec une baisse de 40% des incidents en production après
					refactoring.
				</li>
				<li>
					Amélioration de la maintenabilité : réduction de 15% du code legacy et meilleure
					documentation technique.
				</li>
				<li>
					Collaboration efficace avec les équipes métier et techniques, permettant une amélioration
					continue du produit
				</li>
			</ul>

			{#snippet more()}
				Réalisations :
				<ul class="mt-5 list-inside list-disc">
					<li>
						Développement Fullstack : Implémentation de nouvelles fonctionnalités en frontend et
						backend.
					</li>
					<li>
						Optimisation des performances : Amélioration du temps de réponse des API, optimisation
						du rendu frontend et des requêtes SQL.
					</li>
					<li>
						Gestion des déploiements : Livraison continue et automatisation des mises en production.
					</li>
					<li>
						Audits & refactoring : Analyse du code existant, amélioration de la maintenabilité et
						réduction de la dette technique.
					</li>
					<li>
						Conception technique : Architecture de nouvelles solutions pour répondre aux besoins
						métiers.
					</li>
					<li>Relation client : Collecte des besoin et suivi des évolutions.</li>
				</ul>
			{/snippet}
		</Experience>
		<Experience title="Alten" poste="Développeur Fullstack / DevOps">
			Participation au développement complet d’un outil de gestion des collaborateurs, depuis la
			conception jusqu’au déploiement, en adoptant des technologies modernes et une approche Agile
			(Scrum/Kanban).

			<ul class="mt-5 list-inside list-disc">
				<li>
					Développement accéléré : Lancement de la première version en 4 mois, avec des itérations
					continues.
				</li>

				<li>
					Amélioration de l’expérience utilisateur : Intégration des retours UI/UX permettant une
					adoption rapide par les utilisateurs.
				</li>

				<li>
					Maintenance facilitée : Codebase propre et bien documentée, réduisant la dette technique
					et accélérant l’ajout de nouvelles fonctionnalités.
				</li>
			</ul>

			{#snippet more()}
            Contributions :

            <ul class="mt-5 list-inside list-disc">
                <li>Développement Fullstack : Implémentation du frontend, backend et gestion
                des tâches DevOps.</li>
                <li>Automatisation des déploiements : Mise en place et gestion de pipelines CI/
                CD avec GitLab.</li>
                <li>Architecture logicielle : Conception et modélisation selon le modèle C4,
                assurant une structure évolutive et maintenable.</li>
                <li>Agilité & Collaboration : Participation aux sprints, cérémonies Agile et suivi
                des tâches en équipe.</li>
                <li>Conception UI/UX : Contribution à la définition de l’expérience utilisateur et
                au design des interfaces.</li>
                <li>Livraisons fréquentes : Supervision des déploiements hebdomadaires,
                garantissant un cycle d’amélioration continue.</li>
            </ul>
			{/snippet}
		</Experience>
	</div>
</section>

<section id="projects" class="container mx-auto mt-30">
	<h1 class="my-5 text-center text-3xl font-bold text-[#009688]">Projets</h1>
	<div class="grid gap-5 md:grid-cols-3">
		<Project title="SelfKit" img="selfkit.png" href="https://selfkit.dev" />
		<Project title="Lyky website" img="lyky.png" href="https://practical-mirzakhani-12aa0d.netlify.app/" />
		<Project title="Klape website" img="klape.png" href="https://zealous-mclean-b50936.netlify.app/" />
	</div>
</section>

<section id="contact" class="container mx-auto mt-30">
	<Contact />
</section>
