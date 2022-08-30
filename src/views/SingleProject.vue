<script>
import feather from 'feather-icons';
import ProjectHeader from '../components/projects/ProjectHeader.vue';
import ProjectGallery from '../components/projects/ProjectGallery.vue';
import ProjectInfo from '../components/projects/ProjectInfo.vue';
import ProjectRelatedProjects from '../components/projects/ProjectRelatedProjects.vue';

export default {
	name: 'Projects',
	components: {
		ProjectHeader,
		ProjectGallery,
		ProjectInfo,
		ProjectRelatedProjects,
	},
	data: () => {
		return {
			singleProjectHeader: {
				singleProjectTitle: 'Web Application',
				singleProjectDate: 'Jul 26, 2020',
				singleProjectTag: 'Backend/Frontend',
			},
			projectImages: [
				{
					id: 1,
					title: 'SDF Cambodia',
					img: require('@/assets/images/ui-project-1.jpg'),
				},
				{
					id: 2,
					title: 'SDF Cambodia',
					img: require('@/assets/images/web-project-2.jpg'),
				},
				{
					id: 3,
					title: 'SDF Cambodia',
					img: require('@/assets/images/mobile-project-2.jpg'),
				},
			],
			projectInfo: {
				clientHeading: 'About Client',
				companyInfos: [
					{
						id: 1,
						title: 'MEF',
						details: 'Ministry of Economy and Finance',
					},
					{
						id: 2,
						title: 'Services',
						details: 'Website/Portal',
					},
					{
						id: 3,
						title: 'Website',
						details: 'http://www.sdfcambodia.org/kh/home',
					},
					{
						id: 4,
						title: 'Phone',
						details: 'N/A',
					},
				],
				objectivesHeading: 'Objective',
				objectivesDetails:
					'To be the most trusted financing platform for sustainable and demand-driven skill development.',
				technologies: [
					{
						title: 'Tools & Technologies',
						techs: [
							'HTML',
							'CSS',
							'JavaScript',
							'Laravel',
							'TailwindCSS',
							'MySql',
						],
					},
				],
				projectDetailsHeading: 'Challenge',
				projectDetails: [
					{
						id: 1,
						details:
							'Tens of thousands of Cambodia’s young population enter the labor force each year. Labor force participation among the working age population (15–64 years) increased from 7.7 million in 2009 to 8.3 million in 2015. While the country is endowed with an ample supply of labor, the labor force is still characterized by very low levels of education and skill. The average educational attainment of the current workforce is primary school completion (grade 6) or below—a major barrier to industrial diversification efforts and moving up the value chain. The 2015 Cambodia Socio-Economic Survey found that nearly half (46%) of the labor force have either not completed primary education or never attended school. Less than 7% of workers completed high school (grade 12). There is a pressing need to respond to the growing demand for an adaptable workforce with professional skills and proper workplace behavior. In response, the government has taken steps to reform and strengthen the education and training system, including an enhanced role of the private sector in skills development and providing incentives to enterprises to train their own workforce. The pilot Skills Development Fund (SDF) is an industry-driven workforce development program. The general notion is to build confidence in industry partnership and to engage more strongly with the private sector and their training needs. Firms willing but at times hesitant to further develop their workforce may be supported by the SDF to further invest in workforce development. Motivated private workforce development initiatives and intentions shall be mainly supported by the SDF (which in turn consists of a motivated, skilled, and client-oriented team).',
					}
				
				],
				socialSharingsHeading: 'Share This',
				socialSharings: [
					{
						id: 1,
						name: 'Twitter',
						icon: 'twitter',
						url: 'https://twitter.com/ChhinghorDev',
					},
					{
						id: 2,
						name: 'Instagram',
						icon: 'instagram',
						url: 'https://www.instagram.com/seavhorrr',
					},
					{
						id: 3,
						name: 'Facebook',
						icon: 'facebook',
						url: 'https://facebook.com/stom.sharow',
					},
					{
						id: 4,
						name: 'LinkedIn',
						icon: 'linkedin',
						url: 'https://www.linkedin.com/in/ching-hor-bb7bb415b/',
					},
					{
						id: 5,
						name: 'Youtube',
						icon: 'youtube',
						url: 'https://www.youtube.com/channel/UCSS-bVfkA2CWiAJJjJnUaaQ',
					},
				],
			},
			relatedProject: {
				relatedProjectsHeading: 'Related Projects',
				relatedProjects: [
					{
						id: 1,
						title: 'Mobile UI',
						img: require('@/assets/images/mobile-project-1.jpg'),
					},
					{
						id: 2,
						title: 'Web Application',
						img: require('@/assets/images/web-project-1.jpg'),
					},
					{
						id: 3,
						title: 'UI Design',
						img: require('@/assets/images/ui-project-2.jpg'),
					},
					{
						id: 4,
						title: 'Kabul Mobile App UI',
						img: require('@/assets/images/mobile-project-2.jpg'),
					},
				],
			},
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div class="container mx-auto mt-10 sm:mt-20">
		<!-- Project header -->
		<ProjectHeader :singleProjectHeader="singleProjectHeader" />

		<!-- Project gallery -->
		<ProjectGallery :projectImages="projectImages" />

		<!-- Project information -->
		<ProjectInfo :projectInfo="projectInfo" />

		<!-- Project related projects -->
		<ProjectRelatedProjects :relatedProject="relatedProject" />
	</div>
</template>

<style scoped></style>
