<script lang="ts">
	import Icons from '$lib/components/layout/Icons.svelte';
	import LoadingInPlace from '$lib/components/layout/LoadingInPlace.svelte';
	import type { FeedItem_PostFragmentFragment } from '$lib/graphql/_kitql/graphqlTypes';
	import { addS } from '$lib/utils/formatString';
	import { timeAgo } from '$lib/utils/time-ago';
	import VoteButtons from '../voteButtons/VoteButtons.svelte';

	export let post: FeedItem_PostFragmentFragment | null;
</script>

{#if post}
	<div class="py-1 flex flex-wrap md:flex-nowrap mb-8 border-gray-100 border-b-2">
		<VoteButtons {post} />
		<div class="flex-1 md:flex-grow">
			<a
				href={post?.url}
				class="text-2xl font-medium text-gray-900 hover:text-green-500 title-font mb-2"
			>
				{post.title}
			</a>

			<div class="flex items-center flex-wrap pb-4 border-gray-100 mt-auto w-full">
				<span
					class="text-gray-400 mr-3 inline-flex items-center  text-sm pr-3 py-1 border-r-2 border-gray-200"
				>
					<Icons name="PointIcon" class="w-4 h-4 mr-1" />
					{addS(post.voteTotal, 'point')}
				</span>
				<a
					href={`/item/${post.id}`}
					class="text-gray-400 hover:text-green-400 mr-3 inline-flex items-center text-sm pr-3 py-1 border-r-2 border-gray-200"
				>
					<Icons name="CommentIcon" class="w-4 h-4 mr-1" />
					{addS(post.commentCollection?.totalCount, 'comment')}
				</a>
				<a
					href={`/profile/${post.profile?.id}`}
					class="text-gray-400 hover:text-green-400 mr-3 inline-flex items-center text-sm pr-3 py-1 border-r-2 border-gray-200"
				>
					<img
						class="inline-block h-4 w-4 rounded-full mr-1"
						src={post.profile?.avatarUrl ?? ''}
						alt="avatar"
					/>
					{post.profile?.username}
				</a>
				<a
					href={`/item/${post.id}`}
					class="text-gray-400 hover:text-green-400 inline-flex items-center text-sm"
				>
					<Icons name="CalendarIcon" class="w-4 h-4 mr-1" />
					{timeAgo.format(new Date(post.createdAt))}
				</a>
				<!-- {user?.id && post.profile?.id === user?.id ? (
        <DeleteButton post={post} />
      ) : null} -->
			</div>
		</div>
	</div>
{:else}
	<div class="py-1 flex flex-wrap md:flex-nowrap mb-8 border-gray-100 border-b-2">
		<div class="flex-1 md:flex-grow">
			<span class="text-2xl font-medium text-gray-900 hover:text-green-500 title-font mb-2">
				<LoadingInPlace class="h-8 mb-1" />
			</span>

			<div class="flex items-center flex-wrap pb-4 border-gray-100 mt-auto w-full">
				<span
					class="text-gray-400 mr-3 inline-flex items-center  text-sm pr-3 py-1 border-r-2 border-gray-200"
				>
					<Icons name="PointIcon" class="w-4 h-4 mr-1" />
					{addS(0, 'point')}
				</span>
				<span
					class="text-gray-400 hover:text-green-400 mr-3 inline-flex items-center text-sm pr-3 py-1 border-r-2 border-gray-200"
				>
					<Icons name="CommentIcon" class="w-4 h-4 mr-1" />
					{addS(0, 'comment')}
				</span>
				<span
					class="text-gray-400 hover:text-green-400 mr-3 inline-flex items-center text-sm pr-3 py-1 border-r-2 border-gray-200"
				>
					<span class="inline-block h-4 w-4 rounded-full mr-1 bg-slate-400" />
					{addS(0, 'user')}
				</span>
				<span class="text-gray-400 hover:text-green-400 inline-flex items-center text-sm">
					<Icons name="CalendarIcon" class="w-4 h-4 mr-1" />
					{addS(0, 'days ago')}
				</span>
			</div>
		</div>
	</div>
{/if}
<!-- 


export function FeedItem(props: {
  post: DocumentType<typeof FeedItem_PostFragment>;
}) {
  const { user } = Auth.useUser();
  const createdAt = React.useMemo(
    () => timeAgo.format(new Date(post.createdAt)),
    [post.createdAt]
  );
  return (
    JYCJY
  );
}

const DeleteButton_DeletePostMutation = gql(/* GraphQL */ `
  mutation DeleteButton_DeletePostMutation($postId: BigInt!) {
    deleteFromPostCollection(atMost: 1, filter: { id: { eq: $postId } }) {
      affectedCount
    }
  }
`);

const DeleteButton_PostFragment = gql(/* GraphQL */ `
  fragment DeleteButton_PostFragment on Post {
    id
  }
`);

const DeleteButton = (props: {
  post: DocumentType<typeof DeleteButton_PostFragment>;
}) => {
  const router = useRouter();
  const [show, setShow] = React.useState(false);
  const [deletePostMutation, deletePost] = useMutation(
    DeleteButton_DeletePostMutation
  );

  React.useEffect(() => {
    if (deletePostMutation.data) {
      router.push("/");
    }
  }, [deletePostMutation.data, deletePostMutation.error]);

  return (
    <>
      <button
        class="text-gray-400 hover:text-green-400 inline-flex items-center text-sm pl-3 ml-3 border-l-2 border-gray-200"
        onClick={() => setShow(true)}
      >
        <TrashIcon class="w-4 h-4 mr-1" />
        Delete
      </button>
      <Modal
        title="Do you want to delete your post?"
        visible={show}
        onCancel={() => setShow(false)}
        onConfirm={() => {
          deletePost({
            postId: post.id,
          });
        }}
      >
        Deleting your post can not be reverted
      </Modal>
    </>
  );
}; -->
